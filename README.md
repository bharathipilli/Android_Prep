# Android_Prep
# What is Android?

Android is an operating system mainly used in:

- Smartphones 📱  
- Tablets  
- Smart TVs  
- Cars (Android Automotive)  
- Embedded devices (POS, kiosks, IoT)  

It is **open-source** and based on the **Linux kernel**.

---

## In very simple words

👉 **Android = Linux + Google software + Apps**

- **Linux kernel** → talks to hardware  
- **Android system** → manages phone features  
- **Apps** → what users actually use (WhatsApp, Camera, Maps)

---

## Why Android exists?

Before Android:

- Every phone company had its own OS  
- Apps couldn’t run on different phones  

Android solved this by:

✔ Giving one common OS  
✔ Letting developers write one app that runs on many devices  
✔ Being free and customizable  

---

## Main parts of Android (big picture)
User
↓
Apps (Phone, WhatsApp, YouTube)
↓
Android Framework (Camera, Audio, Location)
↓
Android Runtime (ART)
↓
Hardware Abstraction Layer (HAL)
↓
Linux Kernel (Drivers, Memory, CPU)
↓
Hardware (CPU, RAM, Camera, Sensors)


You don’t need to memorize this yet—just know:  
👉 **Apps never talk directly to hardware**

---

## Is Android Linux?

✔ **Yes and No**

- Uses Linux kernel  
- But not a normal Linux OS like Ubuntu  
- No bash shell by default  
- Uses its own runtime (ART, not glibc)  

So:  
👉 **Android is Linux-based, not Linux desktop**

---

## Key features of Android

- Multitasking (many apps at once)  
- Touch-based UI  
- Strong app sandboxing (apps are isolated)  
- Battery optimized  
- Huge app ecosystem  

---

## Example (real-life analogy)

Think of Android like a company:

- **Linux kernel** → security + workers  
- **Android framework** → managers  
- **Apps** → employees doing actual work  
- **Hardware** → machines in the factory  

---
# What is a Sandbox?

👉 **Sandbox = a safe, isolated area**

In Android:

- Each app runs in its own separate “box”
- One app cannot see or touch another app’s data or memory

---

## Very simple real-life example 🏠

Imagine an apartment building:

- Each flat = one app  

Each flat has:

- Its own room  
- Its own lock  

Neighbors cannot enter your flat without permission.

👉 That flat is the **sandbox**.

---

## In Android terms

When you install an app:

Android gives it:

- Its own memory  
- Its own files  
- Its own user ID (UID)  

So:

- App A ❌ cannot read ❌ App B’s data  
- App B ❌ cannot control ❌ App C  

---

## Why sandbox is needed?

### 1️⃣ Security 🔐

If a virus app is installed:

- Damage is limited to its own sandbox  
- It cannot steal WhatsApp data or banking data  

---

### 2️⃣ Stability 🧱

If one app crashes:

- Other apps keep running  
- Phone does not hang  

---

### 3️⃣ Privacy 👤

Apps cannot:

- Read your photos  
- Access contacts  
- Use camera  

👉 **Unless you allow it**

---

## Then how do apps talk to each other?

Only in controlled ways:

- Permissions (Camera, Contacts, Location)  
- Intents  
- Binder (internal Android IPC)  

So Android says:

> “You can talk, but only through me.”

---

## Very small example

WhatsApp wants camera 📷

Android asks you:

> “Allow camera access?”

- ✔ Allow → WhatsApp can use camera  
- ❌ Deny → Camera blocked  

That permission opens a **small door** in the sandbox.

---

## One-line definition 

**Sandbox is a security mechanism where each Android app runs in an isolated environment to protect system and user data.**

---

