# PF-04: Personal Website Live on the FlyRank Domain

## Student Information

**Name:** Mohd Vasi Saifi  
**Program:** B.Tech (Hons.) Artificial Intelligence & Machine Learning  
**University:** SDGI Global University, Ghaziabad

---

## Live Website

Website URL:

https://vasi-portfolio.netlify.app/

Hosting Platform: Netlify

HTTPS Status: Enabled

---

## Website Purpose

This website serves as my personal portfolio. It includes:

- About Me
- Education
- Skills
- Projects
- Resume
- GitHub Profile
- LinkedIn Profile
- Contact Information

The website is publicly accessible and can be shared with recruiters, mentors, and industry professionals.

---

# DNS Walkthrough

## What is DNS?

DNS (Domain Name System) works like the internet's phonebook. It converts a website name into the server address where the website is hosted.

---

## How My Website Loads

### Step 1

A user enters:

https://vasi-portfolio.netlify.app/

into the browser.

### Step 2

The browser contacts a DNS resolver to find where the website is hosted.

### Step 3

The resolver checks DNS records and identifies that the website is hosted on Netlify.

### Step 4

The DNS system returns the hosting server information to the browser.

### Step 5

The browser connects to the Netlify server using HTTPS.

### Step 6

Netlify provides an SSL certificate that creates a secure encrypted connection.

### Step 7

The website files are delivered from Netlify to the browser.

### Step 8

The browser renders the website and displays the portfolio to the visitor.

---

# Future Custom Domain Setup

When FlyRank provides a custom subdomain such as:

yourname.flyrank.ai

a CNAME record will be created.

Example:

yourname.flyrank.ai → vasi-portfolio.netlify.app

This record tells DNS that the FlyRank domain should point to the Netlify-hosted website.

After DNS propagation and SSL verification, visitors can access the same website through the FlyRank domain.

---

# Website Files

## Main Files

- index.html
- style.css
- script.js

## Assets

- Images
- Resume PDF
- Project Resources

---

# External Links

GitHub:
https://github.com/vasisaifi1-creator

LinkedIn:
https://www.linkedin.com/in/mohdvasisaifi

Portfolio:
https://vasi-portfolio.netlify.app/

---

# Submission Result

The website is successfully deployed on Netlify, accessible through HTTPS, and ready for future FlyRank domain integration.