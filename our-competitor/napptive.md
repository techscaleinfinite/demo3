---
description: >-
  A beacon of simplicity and accessibility in the ever-changing environment of
  cloud-native apps.
cover: ../.gitbook/assets/hNzbbTtx6 (1).png
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Napptive

Using Napptive Playground to Unlock the Power of Kubernetes Napptive Playground stands out as a beacon of simplicity and accessibility in the ever-changing environment of cloud-native apps. With Kubernetes at its foundation, this platform intends to enable users from a variety of disciplines, such as data scientists, business analysts, and modelling specialists, to deploy complex applications with ease while avoiding the complexities of Kubernetes.

<mark style="color:green;">**The Missing Piece: Applications**</mark>

One of the first things Napptive tackles is the concept of "Applications." In the Kubernetes world, this abstraction is somewhat elusive. Users are often left manually piecing together the various components of an application. Napptive recognizes the need for a more straightforward approach, and that's where the Open Application Model (OAM) steps in. OAM provides a universal abstraction for applications, irrespective of the cloud provider, containerization tech, or deployment framework. It's highly customizable, allowing users to add Traits, Policies, or new Component Definitions as needed.

<mark style="color:green;">**KubeVela: Powering Napptive**</mark>

Napptive Playground relies on KubeVela as the OAM runtime for Kubernetes deployments. This innovative approach offers an environment abstraction with multi-tenant capabilities, similar to creating partitions in a shared cluster through distinct namespaces. What sets Napptive apart is its user-friendly configuration that doesn't require in-depth Kubernetes knowledge.

<mark style="color:green;">**A Glimpse of the Architecture**</mark>

Napptive and KubeVela's design is a well-oiled machine when deployed within a Kubernetes cluster. Users can interact with the cluster using the Napptive user interface, which can be accessed via the command line or the web UI. Isolated environments are simple to set up and allow for logical separations depending on deployment type (e.g., deployment, staging, production), purpose (e.g., projectA, projectB), or any other criterion. KubeVela manages the low-level application lifecycle by establishing the appropriate Kubernetes entities after an OAM application is deployed in Kubernetes.

<mark style="color:green;">**A Multi-Tenant Approach**</mark>

Napptive's unique approach lies in its multi-tenant environment. Unlike other KubeVela adopters, Napptive thrives in a multi-user setting. Security is paramount in this setup, and Napptive is dedicated to maintaining multi-tenancy throughout different releases. The focus on RBAC compliance ensures a secure and efficient experience.

<mark style="color:green;">**Napptive's Role in the Community**</mark>

Napptive's journey with the OAM/KubeVela community has evolved from exploration to active contribution. They've worked closely with the core KubeVela development team, testing and overcoming challenges related to multi-tenancy and security. Sharing their perspective and customer use cases, Napptive actively contributes to the growing KubeVela community.

<mark style="color:green;">**A Bright Future Ahead**</mark>

In the future, Napptive Playground offers a hassle-free experience for people interested in exploring the Open Application Model without the need for sophisticated installs. The community contributions continue, with an emphasis on quality assurance tools to assure application stability following upgrades and the adoption of new KubeVela capabilities such as multi-cluster support. Napptive is also aiming towards an OAM-compatible application catalogue, which would ease the storing and accessibility of application definitions. Napptive Playground is a testament to the strength of abstraction and accessibility in the Kubernetes environment, making complicated deployments simple for everybody.

<div>

<figure><img src="../.gitbook/assets/Screenshot 2023-10-05 164644.png" alt=""><figcaption></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Screenshot 2023-10-05 164617.png" alt=""><figcaption></figcaption></figure>

</div>

<mark style="color:purple;">**Check out their website:**</mark>

{% embed url="https://playground.napptive.dev/login" %}
