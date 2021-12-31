# 前序 Eoin Keary

软件的不安全问题也许是我们这个时代最为重要的技术挑战。支持商业、社交网络等 Web 应用程序的急剧增长，只会使建立一种健全的方法来开发和确保我们的 Internet、Web 应用程序和数据安全性的要求更加复杂。

在OWASP团队，我们努力使不安全软件成为这个世界上不正常、不规范的产品。而这份OWASP测试指南正是实现这个目
标的重要一步。通过科学的的理论方法来进行软件测试是非常关键的。我们需要可以重复的、一致性的过程来测试web应
用程序。没有标准的世界是混乱的世界。

毫无疑问的是没有进行过安全测试就无法保证开发出来的是一个安全的应用程序。测试是更广泛的构建安全系统方法的一部分。然而，许多的软件开发组织的标准软件开发流程中却并不包含安全测试这一步骤。更糟糕的是，许多安全供应商提供的测试质量和严格程度各不相同。

由于攻击者能够利用无数的方法来攻破应用程序，而安全测试不可能测试全部的攻击方法，所以安全测试其自身并非是衡量
应用安全最为有效的方法。我们无法破解自己的安全，因为我们只有有限的时间来测试和防御，而攻击者没有这种限制。

结合其他 OWASP 项目，例如代码审查指南、开发指南以及[OWASP ZAP](https://www.zaproxy.org/) 等工具，这是构建和维护安全应用程序的良好开端。本测试指南将向您展示如何验证正在运行的应用程序的安全性。我强烈建议将这些指南用作应用程序安全计划的一部分。

## 为什么需要OWASP？

写成一本这样的指南是艰巨的工作，因为它汇集了数百位世界各地的专家的专业技能。测试安全漏洞有许多不同的方式，但
是这本指南却在如何快捷、准确、有效地测试方面获得了权威人士的一致同意。OWASP 使志同道合的安全人员能够一起工作并形成针对安全问题的领先实践方法。

The importance of having this guide available in a completely free and open way is important for the foundation's mission. It gives anyone the ability to understand the techniques used to test for common security issues. Security should not be a black art or closed secret that only a few can practice. It should be open to all and not exclusive to security practitioners but also QA, Developers and Technical Managers. The project to build this guide keeps this expertise in the hands of the people who need it - you, me and anyone that is involved in building software.

This guide must make its way into the hands of developers and software testers. There are not nearly enough application security experts in the world to make any significant dent in the overall problem. The initial responsibility for application security must fall on the shoulders of the developers because they write the code. It shouldn't be a surprise that developers aren't producing secure code if they're not testing for it or consider the types of bugs which introduce vulnerability.

Keeping this information up to date is a critical aspect of this guide project. By adopting the wiki approach, the OWASP community can evolve and expand the information in this guide to keep pace with the fast moving application security threat landscape.

This Guide is a great testament to the passion and energy our members and project volunteers have for this subject. It shall certainly help to change the world a line of code at a time.

## Tailoring and Prioritizing

You should adopt this guide in your organization. You may need to tailor the information to match your organization's technologies, processes, and organizational structure.

In general there are several different roles within organizations that may use this guide:

- Developers should use this guide to ensure that they are producing secure code. These tests should be a part of normal code and unit testing procedures.
- Software testers and QA should use this guide to expand the set of test cases they apply to applications. Catching these vulnerabilities early saves considerable time and effort later.
- Security specialists should use this guide in combination with other techniques as one way to verify that no security holes have been missed in an application.
- Project Managers should consider the reason this guide exists and that security issues are manifested via bugs in code and design.

The most important thing to remember when performing security testing is to continuously re-prioritize. There are an infinite number of possible ways that an application could fail, and organizations always have limited testing time and resources. Be sure time and resources are spent wisely. Try to focus on the security holes that are a real risk to your business. Try to contextualize risk in terms of the application and its use cases.

This guide is best viewed as a set of techniques that you can use to find different types of security holes. But not all the techniques are equally important. Try to avoid using the guide as a checklist, new vulnerabilities are always manifesting and no guide can be an exhaustive list of "things to test for", but rather a great place to start.

## The Role of Automated Tools

There are a number of companies selling automated security analysis and testing tools. Remember the limitations of these tools so that you can use them for what they're good at. As Michael Howard put it at the 2006 OWASP AppSec Conference in Seattle, "Tools do not make software secure! They help scale the process and help enforce policy."

Most importantly, these tools are generic - meaning that they are not designed for your custom code, but for applications in general. That means that while they can find some generic problems, they do not have enough knowledge of your application to allow them to detect most flaws. In my experience, the most serious security issues are the ones that are not generic, but deeply intertwined in your business logic and custom application design.

These tools can also be very useful, since they do find lots of potential issues. While running the tools doesn't take much time, each one of the potential problems takes time to investigate and verify. If the goal is to find and eliminate the most serious flaws as quickly as possible, consider whether your time is best spent with automated tools or with the techniques described in this guide. Still, these tools are certainly part of a well-balanced application security program. Used wisely, they can support your overall processes to produce more secure code.

## Call to Action

If you're building, designing or testing software, I strongly encourage you to get familiar with the security testing guidance in this document. It is a great road map for testing the most common issues that applications are facing today, but it is not exhaustive. If you find errors, please add a note to the discussion page or make the change yourself. You'll be helping thousands of others who use this guide.

Please consider [joining us](https://owasp.org/membership/) as an individual or corporate member so that we can continue to produce materials like this testing guide and all the other great projects at OWASP.

Thank you to all the past and future contributors to this guide, your work will help to make applications worldwide more secure.

--Eoin Keary, OWASP Board Member, April 19, 2013

Open Web Application Security Project and OWASP are registered trademarks of the OWASP Foundation, Inc.
