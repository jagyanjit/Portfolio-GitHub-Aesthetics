🧩 Portfolio Website — Build Documentation
📘 Overview

This document provides a complete, straightforward breakdown of how your personal portfolio website was built — including layout, structure, features, and the technologies used.
The project is fully hand-coded using HTML, CSS, and JavaScript, with no frameworks or build tools.

⚙️ Core Dependencies
1. Font Awesome (Icons)

Used for all interface and social icons.

<link
  rel="stylesheet"
  href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css"
/>

2. Web3Forms (Contact Form Backend)

Handles form submissions securely without requiring a custom server.

Endpoint:

https://api.web3forms.com/submit

🧱 Structure & Layout

The portfolio follows a dual-panel design for clear separation between navigation and content.

Left Sidebar (<aside class="sidebar">)

Fixed position (width: 380px, height: 100vh)

Independent scroll with overflow-y: auto

Contains:

Profile photo and contact info

Social links

Skills

Education

Contact form

Right Content Area (<main class="main-content">)

Starts after the sidebar (margin-left: 380px)

Independent scroll with overflow-y: auto

Contains:

Projects

Achievements

Certificates

Both panels use a hidden scrollbar (.no-scrollbar) to keep the interface clean.

🧭 Header & Navigation

Two separate headers are used for the dual-panel layout.

Sidebar Header – Displays your name/logo. Clicking it scrolls both panels to the top smoothly.

Main Header – Contains navigation links and the theme toggle.

Navigation links are enhanced with JavaScript for smooth scrolling using custom data-target-* attributes.
This prevents default jumps and adjusts for the fixed header height.

👤 Sidebar Components
Profile

Image:
Profile Picture

Social Links

📞 Phone

💼 LinkedIn

🐙 GitHub

✖️ X (Twitter)

🧩 LeetCode

Skills

Each skill is a clickable badge linking to its official documentation or platform.

| Skill        | Link                                                                                                                   |
| :----------- | :--------------------------------------------------------------------------------------------------------------------- |
| C++          | [https://isocpp.org/](https://isocpp.org/)                                                                             |
| Python       | [https://www.python.org/](https://www.python.org/)                                                                     |
| HTML         | [https://developer.mozilla.org/en-US/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)                 |
| CSS          | [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)                   |
| JavaScript   | [https://developer.mozilla.org/en-US/docs/Web/JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)     |
| AWS          | [https://aws.amazon.com/](https://aws.amazon.com/)                                                                     |
| Docker       | [https://www.docker.com/](https://www.docker.com/)                                                                     |
| Kubernetes   | [https://kubernetes.io/](https://kubernetes.io/)                                                                       |
| Terraform    | [https://www.terraform.io/](https://www.terraform.io/)                                                                 |
| Git/GitHub   | [https://github.com/](https://github.com/)                                                                             |
| CI/CD        | [https://www.redhat.com/en/topics/devops/what-is-ci-cd](https://www.redhat.com/en/topics/devops/what-is-ci-cd)         |
| DevSecOps    | [https://www.redhat.com/en/topics/devops/what-is-devsecops](https://www.redhat.com/en/topics/devops/what-is-devsecops) |
| Scikit-learn | [https://scikit-learn.org/](https://scikit-learn.org/)                                                                 |
| Pandas       | [https://pandas.pydata.org/](https://pandas.pydata.org/)                                                               |
| Keras        | [https://keras.io/](https://keras.io/)                                                                                 |
| NumPy        | [https://numpy.org/](https://numpy.org/)                                                                               |
| TensorFlow   | [https://www.tensorflow.org/](https://www.tensorflow.org/)                                                             |

Education

| Institution                 | Website                                       | Logo                                                                                      |
| :-------------------------- | :-------------------------------------------- | :---------------------------------------------------------------------------------------- |
| Silicon University          | [silicon.ac.in](https://silicon.ac.in/)       | ![Logo](https://drive.google.com/thumbnail?id=1WVmcv47k-PG7B37FUfZ6t-ag7IXfhBt2\&sz=w200) |
| Nayagarh Higher Sec. School | [ngrautocol.ac.in](https://ngrautocol.ac.in/) | ![Logo](https://drive.google.com/thumbnail?id=1dAvwAPbOhWgLqE2okTfpwRxuU4Y1JG-h\&sz=w200) |
| D.A.V. Public School        | [davpuri.org](http://davpuri.org/)            | ![Logo](https://drive.google.com/thumbnail?id=1JVCYbKEl6Hm-Gw8bA1VOthijJ8oJzY5T\&sz=w200) |

Contact Form

Submits directly to your inbox via Web3Forms.

<form action="https://api.web3forms.com/submit" method="POST">
  <input
    type="hidden"
    name="access_key"
    value="c34a790c-ec56-438e-9ed6-02099e52ef76"
  />
</form>

🧩 Projects & Achievements

Projects are displayed in responsive grids with modals for detailed views.

| Project              | Repository / Docs                                                                                                                                                                                 | Preview                                                                                       |
| :------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | :-------------------------------------------------------------------------------------------- |
| Morse Code Converter | [GitHub](https://github.com/jagyanjit/Morse-Code-Converter)                                                                                                                                       | ![Preview](https://vumbnail.com/1122621998.jpg)                                               |
| Mobile App UI        | [GitHub](https://github.com/jagyanjit/Dummy-Mobile-App)                                                                                                                                           | ![Preview](https://vumbnail.com/1122725179.jpg)                                               |
| DevOps Project       | [Repo](https://github.com/jagyanjit/DevopsProject1) / [Docs](https://docs.google.com/document/d/1BrmY6poKK3PfhS8PtQmzWv3cpQSjZQxX/edit?usp=sharing&ouid=102413956562003041794&rtpof=true&sd=true) | ![Preview](https://drive.google.com/thumbnail?id=1MkU47ro2UFx3qxlwVIrXY-ot6cNTj_2b\&sz=w1000) |
| ML Crop Model        | [Notebook](https://github.com/jagyanjit/Machine-Learning-and-Deep-Learning/blob/main/Project_crop.ipynb)                                                                                          | ![Preview](https://drive.google.com/thumbnail?id=1XO2P8jRlKUwItV5bvi2_Qxmk7a4g0GSQ\&sz=w1000) |
| ML Covid Model       | [Notebook](https://github.com/jagyanjit/Machine-Learning-and-Deep-Learning/blob/main/Project_covid.ipynb)                                                                                         | ![Preview](https://drive.google.com/thumbnail?id=1XO2P8jRlKUwItV5bvi2_Qxmk7a4g0GSQ\&sz=w1000) |


Modals display extra information dynamically when users click on cards.
Certificate previews and education logos are displayed in a similar grid layout.

🌗 Theme Toggle

A simple light/dark mode switch built with:

HTML: Checkbox toggle inside a label

CSS: Moves slider and switches icons

JS: Saves theme preference in localStorage

✅ Summary

Fully custom-built using HTML, CSS, and JavaScript

Dual-panel responsive layout

Smooth navigation and accessible UI

Integrated contact form using Web3Forms

Dynamic modals and theme toggle for better UX
