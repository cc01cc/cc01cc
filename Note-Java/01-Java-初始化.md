# 01 Java 初始化-v0.1

> 本文的主要目标是便于后期的回顾，所以会省略部分细节
>
> 操作环境：windows 10, windows 11

## 1. 概览

1. JDK 选择，安装与验证
2. IDE 选择与安装
3. JDK 相关文件

## 2. JDK

> 以下仅为我对于 JDK 选择的倾向，大家可以结合自身需求进行取舍

### 2.1. 选择 JDK

- Redhat OpenJDK 11: <https://developers.redhat.com/products/openjdk/download>
- Microsoft OpenJDK 11: <https://docs.microsoft.com/zh-cn/java/openjdk/download>

#### 2.1.1. 选择 JDK 的参考标准

1. LTS 版本（一般为 Java8, Java11, Java17）
2. 开源，可商用
3. 维护者（平台或社区）的综合实力

#### 2.1.2. 选择 Redhat JDK 主要参考

1. Redhat 是一个相对成熟稳定的平台，并且在开源领域比较有名声。
2. 同时 Redhat 对于 JDK 长期维护的支持与声明，使我比较放心。
3. mi-openjdk-datasheet-f17057cs-201908-a4-zh.pdf : <https://www.redhat.com/rhdc/managed-files/mi-openjdk-datasheet-f17057cs-201908-a4-zh.pdf>

#### 2.1.3. 选择 Microsoft OpenJDK 主要参考

1. Microsoft OpenJDK 下载比较稳定且方便，在一些紧急情况比较合适；（Redhat 需要注册才能下载）
2. Microsoft 这个平台也足够放心

#### 2.1.4. 其他 JDK

1. IBM - Java SDK: <https://www.ibm.com/support/pages/java-sdk/>
2. Amazon Corretto-OpenJDK 的免费多平台发行版-AWS云服务: <https://aws.amazon.com/cn/corretto/>
3. BellSoft - Download OpenJDK builds of Liberica JDK, Java 8, 11, Java 17 Linux, Windows, macOS : <https://bell-sw.com/pages/downloads/#/java-17-lts%20/%20current>
4. Java Downloads | Oracle: <https://www.oracle.com/java/technologies/downloads/>
5. JDK Builds from Oracle: <http://jdk.java.net/>
6. SapMachine | An OpenJDK release maintained and supported by SAP: <https://sap.github.io/SapMachine/>

#### 2.1.5. 其他参考

1. OpenJDK, an open source alternative to Oracle JDK : <https://www.redhat.com/en/resources/build-of-openjdk-datasheet>
2. What Does Long-Term Support Mean for OpenJDK? | Java Code Geeks - 2021 : <https://www.javacodegeeks.com/2019/07/long-term-support-mean-openjdk.html>

#### 2.1.6. JDK 概览

> 这张表格收集的时候忘记记录来源了，数据可能有些过时，可以大致参考

| Provider | Free Builds from Source | Free Binary Distributions | Extended Updates | Commercial Support | Permissive License |
|--|--|--|--|--|--|
| AdoptOpenJDK      |    Yes      |    Yes        |   Yes    |   No       |   Yes      |
| Amazon – Corretto |    Yes      |    Yes        |   Yes    |   No       |   Yes      |
| Azul Zulu         |    No       |    Yes        |   Yes    |   Yes      |   Yes      |
| BellSoft Liberica |    No       |    Yes        |   Yes    |   Yes      |   Yes      |
| IBM               |    No       |    No         |   Yes    |   Yes      |   Yes      |
| jClarity          |    No       |    No         |   Yes    |   Yes      |   Yes      |
| Oracle JDK        |    No       |    Yes        |   No**   |   Yes      |   No       |
| Oracle OpenJDK    |    Yes      |    Yes        |   No     |   No       |   Yes      |
| ojdkbuild         |    Yes      |    Yes        |   No     |   No       |   Yes      |
| RedHat            |    Yes      |    Yes        |   Yes    |   Yes      |   Yes      |
| SapMachine        |    Yes      |    Yes        |   Yes    |   Yes      |   Yes      |

### 2.2. JDK 安装

1. 选择下载压缩包后解压到自己喜欢的文件夹中即可
2. 在系统/用户环境变量中设置 `JAVA_HOME`
   1. `MAVEN` 等程序需要 `JAVA_HOME` 所以不建议省略
3. 将 `bin` 目录添加到系统/用户环境变量的 `Path` 中

### 2.3. JDK 验证

在 `cmd/powershell` 中运行以下命令

```shell
java --version
javac --version
```

## 3. IDE

Java IDE 我一般混合使用 `Eclipse` 和 `IDEA`，两者各有优缺点，可以都尝试一下，不同的开发场景选择合适的工具即可

1. Eclipse IDE for Enterprise Java and Web Developers: <https://www.eclipse.org/downloads/packages/release/2022-06/r/eclipse-ide-enterprise-java-and-web-developers>
2. IntelliJ IDEA: <https://www.jetbrains.com/idea/download/#section=windows>
3. 关于 IDEA 学生可以申请免费的许可证 Free Educational Licenses: <https://www.jetbrains.com/community/education/#students>

## 4. Java 开发相关资料

1. Java Development Kit 11 Documentation: <https://www.oracle.com/java/technologies/javase-jdk11-doc-downloads.html>
2. 嵩山版Java开发手册-阿里云开发者社区: <https://developer.aliyun.com/topic/java20>

## 5. 其他

1. 使用 Git 进行代码的版本控制
   1. Git: <https://git-scm.com/>
2. 我一般选择 Github 作为远程仓库的存储平台
3. 考虑如下：
   1. 平台综合实力成熟度以及认可度较高
   2. 免费的空间以及可用功能更多，以及一些新功能更新的比较快
   3. Github Desktop 使用起来相对顺手方便
   4. GitHub Desktop | Simple collaboration from your desktop: <https://desktop.github.com/>

---

- 署名：cc01cc: <https://github.com/cc01cc>
- 创建并完成于：2022年8月13日
- 关于**转载**
  - 欢迎大家转载分享，转载请标明源地址，切莫破坏或修改原文结构，谢谢
  - 商业转载务必私信通知，非商业转载欢迎私信
  - 在遵守前置规则的条件下，本作品采用[知识共享署名-相同方式共享 4.0 国际许可协议](https://creativecommons.org/licenses/by-sa/4.0/legalcode.zh-Hans)进行许可
- 文章存放并更新自
  - GitHub - cc01cc/cc01cc: <https://github.com/cc01cc/cc01cc>
- TAG: Java JDK Git Github "Github Desktop" Java开发手册 JDK文档 Eclipse IDEA
