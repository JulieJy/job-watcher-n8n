![n8n](https://img.shields.io/badge/n8n-Workflow-orange)
![ATS](https://img.shields.io/badge/ATS-Teamtailor%20%7C%20Ashby-blue)
![Gmail](https://img.shields.io/badge/Gmail-Automation-red)

# 💼 Job Watcher (n8n)

> Automatically monitor multiple ATS providers, filter software engineering job offers matching my profile and receive a daily email digest.

---

## 🎯 Problem solved

Checking multiple company career pages every day is repetitive and time-consuming.

Interesting backend opportunities can easily be missed because each company uses a different Applicant Tracking System (ATS) and exposes its jobs in a different format.

This workflow automatically:
- retrieves job postings from multiple ATS providers,
- normalizes them into a common schema,
- filters only recent software engineering opportunities,
- delivers a daily email with the jobs matching my profile.

---

## 🇫🇷 Présentation

Ce projet est un workflow **n8n** qui automatise la veille d'offres d'emploi.

Chaque jour, il :

- 🏢 Récupère les offres depuis plusieurs ATS (Teamtailor, Ashby)
- 🔄 Normalise les données dans un format commun
- 📅 Conserve uniquement les offres récentes
- 🎯 Filtre les postes correspondant à mon profil
- 📧 Génère un e-mail HTML récapitulatif et l'envoie automatiquement

Ce projet a été réalisé pour découvrir **n8n**, expérimenter l'orchestration de workflows et construire un système de veille d'emploi facilement extensible à de nouveaux ATS.

---

## 🇬🇧 Overview

This project is an **n8n** workflow that automates job monitoring across multiple Applicant Tracking Systems.

Every day it:

- 🏢 Fetches job postings from multiple ATS providers (Teamtailor, Ashby)
- 🔄 Normalizes them into a common schema
- 📅 Keeps only recently published jobs
- 🎯 Filters roles matching my profile
- 📧 Generates and sends a polished HTML email summary

The goal of this project is to explore **n8n**, workflow orchestration and build an extensible job monitoring pipeline supporting multiple ATS providers.

---

## ⚙️ Workflow

![Workflow](screenshots/job-watcher-workflow.png)

---

## 🔎 Supported ATS

- Teamtailor (JSON Feed)
- Ashby

The workflow is designed to be easily extended with additional ATS providers by simply adding a new normalization branch.

---

## 🛠️ Tech Stack

- n8n
- JavaScript
- Gmail
- Teamtailor JSON Feed
- Ashby API

---

## 📸 Example email

![Workflow](screenshots/job-watcher-email.png)

---

## 🚀 Future Improvements

- Support additional ATS providers (Greenhouse, Lever, Workday...)
- Store previously notified jobs to avoid duplicate emails
- Add semantic filtering using an LLM
- Generate personalized cover letter suggestions

---

## 💡 Why I built this

I wanted to learn **n8n** by building a real-world automation that I actually use.

Rather than checking dozens of company career pages manually every day, I chose to automate the entire process and create a reusable pipeline capable of supporting multiple ATS providers.

---

## 💭 What I learned

- Building production-ready workflows with n8n
- Working with multiple ATS providers
- Normalizing heterogeneous API responses into a common schema
- Building reusable workflow branches
- Automating daily notifications with Gmail
