---
description: >-
  Four typical types of scenarios for Layer 2 and Layer 3 networks are described
  as follows.
---

# Scenarios

## Layer 2 Network​

| Scenario         | Fabric​ (Backbone) | Access (Last Mile) | Access (Last Mile) | Access (Last Mile) | OnRamp​ (First Mile) |
| ---------------- | ------------------ | ------------------ | ------------------ | ------------------ | -------------------- |
|                  | Private Connect​   | Port               | Cross Connect      | Local Loop         | Cloud Connect​       |
| IDC to IDC​      | √                  | √                  | √                  |                    |                      |
| Office to IDC​   | √                  | √                  | √                  | √                  |                      |
| IDC to Cloud​    | √                  | √                  | √                  |                    | √                    |
| Office to Cloud​ | √                  | √                  |                    | √                  | √                    |

## Layer 3 Network

| Scenario         | Fabric​ (Backbone) | Access (Last Mile) | Access (Last Mile) | Access (Last Mile) | Access (Last Mile) | OnRamp​ (First Mile) |
| ---------------- | ------------------ | ------------------ | ------------------ | ------------------ | ------------------ | -------------------- |
|                  | Cloud Router​      | Port               | Cross Connect      | Local Loop         | Virtual Edge       | Cloud Connect​       |
| IDC to IDC​      | √                  | √                  | √                  |                    |                    |                      |
| Office to IDC​   | √                  | √                  | √                  |                    | √                  |                      |
| IDC to Cloud​    | √                  | √                  | √                  |                    |                    | √                    |
| Office to Cloud​ | √                  |                    |                    |                    | √                  | √                    |

{% hint style="info" %}
<mark style="color:blue;">**Note**</mark>

* <mark style="color:blue;">IDC refers to Internet Data Center.</mark>
* <mark style="color:blue;">If your data center is too far to establish cross connect to the equipment port in our SDN POP, you can choose to deploy a local loop.</mark>
{% endhint %}

****
