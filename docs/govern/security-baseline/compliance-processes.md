---
title: Security Baseline policy compliance processes
description: Learn an approach to creating processes that support a Security Baseline discipline.
author: martinekuan
ms.author: martinek
ms.date: 09/17/2019
ms.topic: conceptual
ms.service: cloud-adoption-framework
ms.subservice: govern
ms.custom: internal
---

# Security Baseline policy compliance processes

This article discusses an approach to policy adherence processes that govern the [Security Baseline discipline](./index.md). Effective governance of cloud security starts with recurring manual processes. These processes are designed to detect vulnerabilities and impose policies to remediate those security risks. Using these processes requires that the cloud governance team and interested business and IT stakeholders regularly review and update policies and ensure policy compliance. Many ongoing monitoring and enforcement processes can also be automated or supplemented with tooling. This practice reduces the overhead of governance and allows for faster response to policy deviation.

## Planning, review, and reporting processes

The best Security Baseline tools in the cloud are only as good as the processes and policies that they support. The following example processes are commonly involved in the Security Baseline discipline. They can be a good resource when you update your security policy. Typically, you update your policy based on business change and feedback. The feedback comes from security and IT teams that are tasked with turning governance guidance into action. Use these examples as a starting point when you update your policy.

**Initial risk assessment and planning:** As part of your initial adoption of the Security Baseline discipline, identify your core business risks and tolerances that are related to cloud security. Use this information to discuss specific technical risks with members of your IT and security teams. As part of that discussion, establish your initial governance strategy by developing a baseline set of security policies for mitigating these risks.

**Deployment planning:** Before you deploy any workload or asset, perform a security review. In that review, identify any new risks, and ensure all access and data security policy requirements are met.

**Deployment testing:** When you deploy a workload or asset, review the deployment to validate security policy compliance. Make the cloud governance team responsible for that review in cooperation with your corporate security teams.

**Annual planning:** On an annual basis, perform a high-level review of Security Baseline strategy. Explore future corporate priorities and updated cloud adoption strategies to identify potential risk increase and other emerging security needs. Also review the latest security baseline best practices, and integrate these practices into your policies and review processes.

**Quarterly review and planning:** On a quarterly basis, review security audit data and incident reports. Identify any changes that are required in security policy. As part of this process, review the current cybersecurity landscape to proactively anticipate emerging threats. Update your policy as appropriate. After the review is complete, align design guidance with the updated policy.

This planning process is also a good time to evaluate the current membership of your cloud governance team. Look for knowledge gaps that are related to new or changing policies. Also look for risks that are related to security. Invite relevant IT staff to participate in reviews and planning as either temporary technical advisors or permanent members of your team.

**Education and training:** On a bimonthly basis, offer training sessions to make sure IT staff and developers are up to date on the latest security policy requirements. As part of this process, review and update any documentation, guidance, or other training assets. Ensure that they're in sync with the latest corporate policy statements.

**Monthly audit and reporting reviews:** On a monthly basis, perform an audit on all cloud deployments to assure their continued alignment with security policy. Review security-related activities with IT staff. Identify any compliance issues that aren't already handled as part of the ongoing monitoring and enforcement process. Produce a report as the result of this review. Distribute that report to the cloud strategy team and each cloud adoption team to communicate overall adherence to policy. Store the report for auditing and legal purposes.

## Processes for ongoing monitoring

The success of a Security Baseline strategy depends on its visibility into the current and past state of your cloud infrastructure. You need to be able to analyze the relevant metrics and data of the security health and activity of your cloud resources. Without this information, you can't identify changes in your risks or detect violations of your risk tolerances. Ongoing governance processes require high-quality data. Only then can you ensure that you can modify policies to better protect your infrastructure against changing threats and security requirements.

Ensure that your security and IT teams have implemented automated monitoring systems for your cloud infrastructure. Make sure that these systems capture the log data that you need to evaluate risk. Be proactive in monitoring these systems to ensure prompt detection and mitigation of potential policy violation. Ensure your monitoring strategy is in line with security needs.

## Violation triggers and enforcement actions

Security noncompliance can lead to critical data exposure and service disruptions. To lower these risks, give the cloud governance team visibility into serious policy violations. Ensure that IT staff has clear escalation paths for reporting security issues. Also ensure that those escalation reports go to the governance team members who are best suited to identify and verify that policy issues are mitigated.

When you detect violations, take action to realign with your policy as soon as possible. Your IT team can automate most violation triggers by using the tools outlined in the [Security Baseline toolchain for Azure](./toolchain.md).

The following triggers and enforcement actions provide examples that you can reference when you plan how to use monitoring data to resolve policy violations:

- **Increase in attacks detected.** If any resource experiences a 25 percent increase in brute force or DDoS attacks, discuss the situation with IT security staff and the workload owner to determine remedies. Track the issue, and update your guidance if you need to revise policies to mitigate future incidents.
- **Unclassified data detected.** If a data source doesn't have an appropriate privacy, security, or business impact classification, deny it external access. Grant access only when the data owner applies the classification and an appropriate level of data protection.
- **Security health issue detected.** Disable access to any virtual machines (VMs) that have known access or malware vulnerabilities. Grant access only after you have installed appropriate patches or security software. Update policy guidance to account for any newly detected threats.
- **Network vulnerability detected.** Configure your system to send an alert whenever a resource is accessed that network access policies don't explicitly allow. Send the alert to IT security staff and the relevant workload owner. Track the issue, and update your guidance if you need to revise policies to mitigate future incidents.

## Next steps

Use the [Security Baseline discipline template](./template.md) to document the processes and triggers that align with the current cloud adoption plan.

For guidance on executing cloud management policies in alignment with adoption plans, see the following article on discipline improvement.

> [!div class="nextstepaction"]
> [Security Baseline discipline improvement](./discipline-improvement.md)
