
# Deptree:

<h2 style="color: black;"> Automate OSS Compliance Work in Yocto Projects</h2>

---

## FOSSology

- it is a powerful tool, but many processes must be run manually, file-by-file, package-by-package
- luckily, there are some CLI tools

---

## Yocto

- are you all familiar with Yocto?
- if you want to bake, you need recipes
- hw manufacturers do not provide ad-hoc linux distros but Yocto recipes
- only a fraction of OSS source code fetched by Yocto ends up in firmware
- manually finding (hundreds of) relevant packages and uploading them to FOSSology: a crazy task

---

### Technical Context

- Linux Embedded project with custom/proprietary code written in C/C++
- dependencies: only static and dynamic linking
- don't touch the compiling machine! 

---

### Legal Context

- proprietary/custom packages ("own packages") and dependencies of own packages deserve a more in depth analysis than "mere-aggregation" packages
- conflicts with OSS (Copyleft) licenses are more likely to happen with proprietary/custom packages (no public scrutiny)

---

### How it works, in practice (1)

- Snapshot of Yocto build dir, copied to a dedicated FOSSology machine (with Deptree)
- Automatic BAT scan
- Automatic detection of dynamic deps for each binary file
- Automatic detection of each binary file's package

---

### How it works, in practice (2)

- Mark "own" packages
- Automatic detection of dependencies of own packages and "mere-aggregation" packages
- Automatic upload of all packages to FOSSology, already organized in folders by project -> version -> category (own/deps-of-own/mere-aggregation)
- Automatic schedule of FOSSology scan/bulk agents for all packages (include reuse of previous clearing decisions)

---

### How it works, in practice (3)

- license clearing of deltas with respect to previous versions of the same project
- manually spot and mark static dependencies
- Any legal issues?
- Automatic sync of FOSSology results with Deptree 
- present results in a simple and meaningful way

---
### Let's see it in action

---
### TODO

- continuous integration in the build process; 
- enable implementation of company's internal OSS policies
- modularity and independency from any specific tool
-
- 
- create an internal DB 

- automatic snapshot and copy of yocto build dir on FOSSology machine
- automatic detection of static dependencies
- license mapping at binary level (and not only at package level)
- should we use also other license scan tools? Scancode?
- create own db of licenses (SPDX) and stuff (avoid links to fossology pages)
- a better name?

---
@title[Copyright and License]
<div class="bottom">
@fa[copyright fa-red] 2018 - Alberto Pianon; Carlo Piana (some rights reserved)   
Licenza Creative Commons by-ND-NC 4.0 unported.  

<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>.

<p>produced with [Gitpitch](https://gitpitch.com/) e [Reveal.js][81aa3153]</p>

</div>

  [81aa3153]: https://revealjs.com/ "Reveal"
