# 🧪 Lab: CloudFormation — 10 EC2 + Application Load Balancer

Laboratorio práctico de AWS CloudFormation donde desplegarás una infraestructura completa con **10 instancias EC2** distribuidasen dos zonas de disponibilidad, todas detrás de un **Application Load Balancer (ALB)** en una VPC dedicada.

---

## 📐 Arquitectura

```
Internet
   │
   ▼
[Application Load Balancer]
   │            │
   ▼            ▼
Subnet-1     Subnet-2
(AZ-a)       (AZ-b)
  │              │
EC2-01        EC2-02
EC2-03        EC2-04
EC2-05        EC2-06
EC2-07        EC2-08
EC2-09        EC2-10
```

---

## ✅ Prerrequisitos

- Cuenta de AWS activa
- Permisos de IAM para: `EC2`, `CloudFormation`, `ElasticLoadBalancing`, `VPC`
- Un **Key Pair** creado previamente en la región donde desplegarás
- AWS CLI configurada *(opcional, para despliegue por consola)*

---

## 📁 Archivos del laboratorio

```
.
├── Laboratorio2.yml   ← Plantilla CloudFormation (este archivo)
└── README.md         ← Este documento
```

## 🗺️ Regiones soportadas

La plantilla incluye AMIs de Amazon Linux para la siguiente región:

| Región         | Código          |
|----------------|-----------------|
| Ohio           | `us-east-2`     |

---

