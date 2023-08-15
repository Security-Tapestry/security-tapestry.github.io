---
title: Threat Detection for Amazon S3 | AI-Powered Data Protection
categories: [Vulnerabilities/Threats]
tags: [threat,detection,amazon,aws,s3,sentinelone]
render_with_liquid: false
# image: /assets/img/dataleak.webp
date: 2023-08-15 12:25 PM
---

SentinelOne recently announced the launch of the new Singularity™ Cloud Data Security product line to help customers gain visibility and provide protection for their cloud data, storage, downstream applications, and users from risks associated with unscanned files. Threat Protection for NetApp provides protection for NetApp arrays, and Threat Detection for Amazon S3, which will be highlighted here, provides protection for S3 buckets. Both services provide powerful, low-latency security for cloud storage in a highly efficient and simple user experience.

### Why Does Amazon S3 Require Protection?

Amazon S3 is one of the most commonly used AWS services. Due to its flexible, scalable, and available nature, it is possible to store and access nearly any object type from anywhere. With this flexibility, there are a variety of use cases for the service, but in today’s environments, we see Amazon S3 being used more by applications than by humans looking for storage. S3 buckets being used by applications house critical application data for apps themselves but also sensitive data. Uptime and performance are mission critical.

Earlier this year, Amazon S3 turned 17 years old, and AWS shared that it currently holds more than 280 trillion objects and has an average of over 100 million requests per second. As part of the shared responsibility model, AWS ensures that the infrastructure itself is secure, and even ensures data integrity within S3. However, the security of what is in the bucket and its potential spread to downstream applications or workflows is the responsibility of the customer.

Many Amazon S3 users and security teams think of configuration management as the primary security challenge, and this used to be a bigger issue with buckets with sensitive data accidentally made public. AWS, though, has implemented new measures to encourage proper configuration. To combat this data loss risk,  many organizations use a Cloud Security Posture Management (CSPM) solution to scan for potential misconfigurations, which is an important element of a defense-in-depth strategy. However, CSPM alone is not enough to prevent S3 from being an attack surface.

The sheer volume of data stored in S3, most of it unscanned and accessible to downstream applications and workflows (including user endpoints), poses a security risk to organizations in terms of malware, ransomware, remote access trojans (RATs), supply chain attacks, and more. Without additional protection, an organization’s S3 buckets can become an accidental staging area for malware.

### Threat Detection for Amazon S3

With Threat Detection for Amazon S3, organizations can decrease risk and increase visibility when it comes to the objects in their buckets. Reducing risk is important and so is meeting compliance requirements including data sovereignty. The solution was designed to meet the business, security, and cloud architecture needs of customers, focusing on the following features:

* AI-Driven Threat Detection – Powerful, AI-driven threat detection goes beyond traditional signature-based approaches, which are easily evaded, and protects the organization from threats faster.
* Automation, Flexibility, and Scalability – Scan new files added to buckets automatically. Inventory and protect buckets, including new buckets automatically as they are created, based on configurable policy based approaches.
* High Performance, Low Overhead – Easily deploy into cloud-native architectures using CloudFormation Templates with low ongoing overhead and minimal additional compute costs. Files are scanned quickly, keeping applications running smoothly.
* Compliance-Ready – Scanning completed in customer cloud; no sensitive data or files leave the organization’s cloud environment.
* Centralized Management Experience – Delivered in a simple, unified management experience within the SentinelOne console, where customers can also manage the protection of cloud workloads, endpoints, and identity.

Existing solutions in the market have left many customers frustrated due to poor security performance such as a signature-only approach and a lack of visibility into the resources and their protection status. Other challenges include sluggish scanning or unnatural deployment patterns that slow applications down, or require time consuming re-architecture.

### Simple, Powerful Security For Simple Storage Service

Configuration scanning is not enough – danger resides in the data itself, being passed downstream. The popularity and flexibility of Amazon S3 leads to a potentially broad attack surface for many organizations that have not begun scanning and securing the data residing in their buckets. Regardless of cloud maturity or S3 use cases, organizations now have a simple and scalable solution to protect their data, their users, and their businesses with Threat Detection for Amazon S3.

Simple deployment, powerful AI-driven threat detection and response with in-line and in-bucket scanning will enable customers to protect their Amazon S3 buckets, critical business applications, and users from malware, ransomware, remote access trojans (RATs) and more.