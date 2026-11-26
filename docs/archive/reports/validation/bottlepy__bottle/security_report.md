# Security Analysis Report

**Target:** `bottlepy/bottle`  
**Scan Date:** 2026-01-07 07:04:03 UTC  
**Scan ID:** `scan-20260107-070355-89f02b34`
**Commit:** `62ca0c31987e`
**Primary Language:** Python
**GitHub Stars:** 8,725

---

## Executive Summary

**Overall Risk Level:** 🟠 **HIGH** - Significant issues found

This security scan analyzed `bottlepy/bottle` and identified **311 potential security issues**.

### Findings by Severity

| Severity | Count | Action Required |
|----------|-------|-----------------|
| 🟠 High | 11 | Soon |
| 🟢 Low | 300 | When convenient |

### Findings by Category

- 📝 **Typos & Code Quality**: 300 issue(s)
- 🔐 **Exposed Secrets & Credentials**: 11 issue(s)

---

## Severity Rating Guide

| Level | Meaning | Response Time |
|-------|---------|---------------|
| 🔴 Critical | Exploitable vulnerability with severe impact | Immediate (hours) |
| 🟠 High | Serious issue requiring prompt attention | Days |
| 🟡 Medium | Moderate risk, should be planned | Weeks |
| 🟢 Low | Minor issue, low risk | When convenient |

---

## Findings Overview

| # | Severity | Category | Title | Location |
|---|----------|----------|-------|----------|
| 1 | 🟢 | Typo | Typo: 'childs' | `bottle.py:752` |
| 2 | 🟢 | Typo | Typo: 'build-in' | `bottle.py:2475` |
| 3 | 🟢 | Typo | Typo: 'clen' | `bottle.py:2814` |
| 4 | 🟢 | Typo | Typo: 'clen' | `bottle.py:2820` |
| 5 | 🟢 | Typo | Typo: 'clen' | `bottle.py:2840` |
| 6 | 🟢 | Typo | Typo: 'clen' | `bottle.py:2845` |
| 7 | 🟢 | Typo | Typo: 'cutted' | `bottle.py:3201` |
| 8 | 🟢 | Typo | Typo: 're-use' | `bottle.py:4212` |
| 9 | 🟢 | Typo | Typo: 'loosly' | `docs\changelog.rst:8` |
| 10 | 🟢 | Typo | Typo: 'Whats' | `docs\changelog.rst:211` |
| 11 | 🟢 | Typo | Typo: 'deprectated' | `docs\deployment.rst:77` |
| 12 | 🟢 | Typo | Typo: 'absolut' | `docs\faq.rst:41` |
| 13 | 🟢 | Typo | Typo: 'appropiate' | `docs\faq.rst:271` |
| 14 | 🟢 | Typo | Typo: 'ist' | `docs\tutorial.rst:156` |
| 15 | 🟢 | Typo | Typo: 'absolut' | `docs\tutorial.rst:277` |
| 16 | 🟢 | Typo | Typo: 'appropiate' | `docs\tutorial.rst:659` |
| 17 | 🟢 | Typo | Typo: 'publically' | `docs\tutorial_app.rst:33` |
| 18 | 🟢 | Typo | Typo: 'validtion' | `docs\tutorial_app.rst:33` |
| 19 | 🟢 | Typo | Typo: 'formated' | `docs\tutorial_app.rst:52` |
| 20 | 🟢 | Typo | Typo: 'build-in' | `docs\tutorial_app.rst:149` |
| 21 | 🟢 | Typo | Typo: 'formated' | `docs\tutorial_app.rst:200` |
| 22 | 🟢 | Typo | Typo: 'build-in' | `docs\tutorial_app.rst:238` |
| 23 | 🟢 | Typo | Typo: 'couse' | `docs\tutorial_app.rst:317` |
| 24 | 🟢 | Typo | Typo: 'similat' | `docs\tutorial_app.rst:473` |
| 25 | 🟢 | Typo | Typo: 'relativ' | `docs\tutorial_app.rst:532` |
| 26 | 🟢 | Typo | Typo: 'build-in' | `docs\tutorial_app.rst:551` |
| 27 | 🟢 | Typo | Typo: 'modifiying' | `docs\tutorial_app.rst:579` |
| 28 | 🟢 | Typo | Typo: 'build-in' | `docs\tutorial_app.rst:605` |
| 29 | 🟢 | Typo | Typo: 'excuted' | `docs\tutorial_app.rst:616` |
| 30 | 🟢 | Typo | Typo: 'build-in' | `docs\tutorial_app.rst:621` |
| 31 | 🟢 | Typo | Typo: 'build-in' | `docs\tutorial_app.rst:623` |
| 32 | 🟢 | Typo | Typo: 'build-in' | `docs\tutorial_app.rst:627` |
| 33 | 🟢 | Typo | Typo: 'utilizin' | `docs\tutorial_app.rst:669` |
| 34 | 🟢 | Typo | Typo: 're-usable' | `docs\plugins\index.rst:13` |
| 35 | 🟢 | Typo | Typo: 'Referenz' | `docs\_locale\de_DE\LC_MESSAGES\api.po:24` |
| 36 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\api.po:30` |
| 37 | 🟢 | Typo | Typo: 'childs' | `docs\_locale\de_DE\LC_MESSAGES\api.po:624` |
| 38 | 🟢 | Typo | Typo: 'accpets' | `docs\_locale\de_DE\LC_MESSAGES\changelog.po:498` |
| 39 | 🟢 | Typo | Typo: 'Whats' | `docs\_locale\de_DE\LC_MESSAGES\changelog.po:521` |
| 40 | 🟢 | Typo | Typo: 'modue' | `docs\_locale\de_DE\LC_MESSAGES\configuration.po:226` |
| 41 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\contact.po:50` |
| 42 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\contact.po:64` |
| 43 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\contact.po:66` |
| 44 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\contact.po:66` |
| 45 | 🟢 | Typo | Typo: 'Dokument' | `docs\_locale\de_DE\LC_MESSAGES\development.po:30` |
| 46 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:30` |
| 47 | 🟢 | Typo | Typo: 'Wege' | `docs\_locale\de_DE\LC_MESSAGES\development.po:40` |
| 48 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\development.po:53` |
| 49 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\development.po:60` |
| 50 | 🟢 | Typo | Typo: 'als' | `docs\_locale\de_DE\LC_MESSAGES\development.po:99` |
| 51 | 🟢 | Typo | Typo: 'Archiv' | `docs\_locale\de_DE\LC_MESSAGES\development.po:99` |
| 52 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\development.po:99` |
| 53 | 🟢 | Typo | Typo: 'Paket' | `docs\_locale\de_DE\LC_MESSAGES\development.po:118` |
| 54 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:128` |
| 55 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\development.po:128` |
| 56 | 🟢 | Typo | Typo: 'alle' | `docs\_locale\de_DE\LC_MESSAGES\development.po:128` |
| 57 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\development.po:128` |
| 58 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\development.po:140` |
| 59 | 🟢 | Typo | Typo: 'deine' | `docs\_locale\de_DE\LC_MESSAGES\development.po:140` |
| 60 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\development.po:155` |
| 61 | 🟢 | Typo | Typo: 'hart' | `docs\_locale\de_DE\LC_MESSAGES\development.po:155` |
| 62 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:155` |
| 63 | 🟢 | Typo | Typo: 'Applikation' | `docs\_locale\de_DE\LC_MESSAGES\development.po:167` |
| 64 | 🟢 | Typo | Typo: 'offen' | `docs\_locale\de_DE\LC_MESSAGES\development.po:178` |
| 65 | 🟢 | Typo | Typo: 'sie' | `docs\_locale\de_DE\LC_MESSAGES\development.po:178` |
| 66 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:186` |
| 67 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:196` |
| 68 | 🟢 | Typo | Typo: 'Alle' | `docs\_locale\de_DE\LC_MESSAGES\development.po:196` |
| 69 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:211` |
| 70 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:211` |
| 71 | 🟢 | Typo | Typo: 'als' | `docs\_locale\de_DE\LC_MESSAGES\development.po:211` |
| 72 | 🟢 | Typo | Typo: 'Alle' | `docs\_locale\de_DE\LC_MESSAGES\development.po:222` |
| 73 | 🟢 | Typo | Typo: 'sie' | `docs\_locale\de_DE\LC_MESSAGES\development.po:222` |
| 74 | 🟢 | Typo | Typo: 'Thats' | `docs\_locale\de_DE\LC_MESSAGES\development.po:233` |
| 75 | 🟢 | Typo | Typo: 'branche' | `docs\_locale\de_DE\LC_MESSAGES\development.po:235` |
| 76 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:235` |
| 77 | 🟢 | Typo | Typo: 'Ende' | `docs\_locale\de_DE\LC_MESSAGES\development.po:235` |
| 78 | 🟢 | Typo | Typo: 'deine' | `docs\_locale\de_DE\LC_MESSAGES\development.po:267` |
| 79 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:267` |
| 80 | 🟢 | Typo | Typo: 'deine' | `docs\_locale\de_DE\LC_MESSAGES\development.po:267` |
| 81 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:267` |
| 82 | 🟢 | Typo | Typo: 'alle' | `docs\_locale\de_DE\LC_MESSAGES\development.po:281` |
| 83 | 🟢 | Typo | Typo: 'applyed' | `docs\_locale\de_DE\LC_MESSAGES\development.po:286` |
| 84 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\development.po:288` |
| 85 | 🟢 | Typo | Typo: 'deine' | `docs\_locale\de_DE\LC_MESSAGES\development.po:288` |
| 86 | 🟢 | Typo | Typo: 'sie' | `docs\_locale\de_DE\LC_MESSAGES\development.po:288` |
| 87 | 🟢 | Typo | Typo: 'als' | `docs\_locale\de_DE\LC_MESSAGES\development.po:288` |
| 88 | 🟢 | Typo | Typo: 'deine' | `docs\_locale\de_DE\LC_MESSAGES\development.po:288` |
| 89 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\development.po:295` |
| 90 | 🟢 | Typo | Typo: 'passt' | `docs\_locale\de_DE\LC_MESSAGES\development.po:295` |
| 91 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:306` |
| 92 | 🟢 | Typo | Typo: 'manuell' | `docs\_locale\de_DE\LC_MESSAGES\development.po:306` |
| 93 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:317` |
| 94 | 🟢 | Typo | Typo: 'Als' | `docs\_locale\de_DE\LC_MESSAGES\development.po:325` |
| 95 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:325` |
| 96 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:333` |
| 97 | 🟢 | Typo | Typo: 'lokal' | `docs\_locale\de_DE\LC_MESSAGES\development.po:333` |
| 98 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:342` |
| 99 | 🟢 | Typo | Typo: 'deine' | `docs\_locale\de_DE\LC_MESSAGES\development.po:342` |
| 100 | 🟢 | Typo | Typo: 'sie' | `docs\_locale\de_DE\LC_MESSAGES\development.po:342` |
| 101 | 🟢 | Typo | Typo: 'deine' | `docs\_locale\de_DE\LC_MESSAGES\development.po:342` |
| 102 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:349` |
| 103 | 🟢 | Typo | Typo: 'sie' | `docs\_locale\de_DE\LC_MESSAGES\development.po:361` |
| 104 | 🟢 | Typo | Typo: 'sie' | `docs\_locale\de_DE\LC_MESSAGES\development.po:361` |
| 105 | 🟢 | Typo | Typo: 'alle' | `docs\_locale\de_DE\LC_MESSAGES\development.po:367` |
| 106 | 🟢 | Typo | Typo: 'committe' | `docs\_locale\de_DE\LC_MESSAGES\development.po:367` |
| 107 | 🟢 | Typo | Typo: 'deine' | `docs\_locale\de_DE\LC_MESSAGES\development.po:367` |
| 108 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:383` |
| 109 | 🟢 | Typo | Typo: 'deine' | `docs\_locale\de_DE\LC_MESSAGES\development.po:383` |
| 110 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:383` |
| 111 | 🟢 | Typo | Typo: 'alle' | `docs\_locale\de_DE\LC_MESSAGES\development.po:383` |
| 112 | 🟢 | Typo | Typo: 'committe' | `docs\_locale\de_DE\LC_MESSAGES\development.po:383` |
| 113 | 🟢 | Typo | Typo: 'als' | `docs\_locale\de_DE\LC_MESSAGES\development.po:389` |
| 114 | 🟢 | Typo | Typo: 'deine' | `docs\_locale\de_DE\LC_MESSAGES\development.po:389` |
| 115 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:398` |
| 116 | 🟢 | Typo | Typo: 'deine' | `docs\_locale\de_DE\LC_MESSAGES\development.po:398` |
| 117 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:414` |
| 118 | 🟢 | Typo | Typo: 'Branche' | `docs\_locale\de_DE\LC_MESSAGES\development.po:420` |
| 119 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\development.po:430` |
| 120 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\development.po:436` |
| 121 | 🟢 | Typo | Typo: 'Ist' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:32` |
| 122 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:43` |
| 123 | 🟢 | Typo | Typo: 'sie' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:43` |
| 124 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:43` |
| 125 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:43` |
| 126 | 🟢 | Typo | Typo: 'Probleme' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:47` |
| 127 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:59` |
| 128 | 🟢 | Typo | Typo: 'Probleme' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:81` |
| 129 | 🟢 | Typo | Typo: 'Adresse' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:91` |
| 130 | 🟢 | Typo | Typo: 'lokal' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:91` |
| 131 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:91` |
| 132 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:91` |
| 133 | 🟢 | Typo | Typo: 'lokale' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:91` |
| 134 | 🟢 | Typo | Typo: 'deines' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:91` |
| 135 | 🟢 | Typo | Typo: 'Proxys' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:91` |
| 136 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\faq.po:91` |
| 137 | 🟢 | Typo | Typo: 'informations' | `docs\_locale\de_DE\LC_MESSAGES\plugindev.po:212` |
| 138 | 🟢 | Typo | Typo: 'infastructure' | `docs\_locale\de_DE\LC_MESSAGES\recipes.po:291` |
| 139 | 🟢 | Typo | Typo: 'Ende' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:37` |
| 140 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:37` |
| 141 | 🟢 | Typo | Typo: 'als' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:37` |
| 142 | 🟢 | Typo | Typo: 'Referenz' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:37` |
| 143 | 🟢 | Typo | Typo: 'Sie' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:37` |
| 144 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:37` |
| 145 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:37` |
| 146 | 🟢 | Typo | Typo: 'alle' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:57` |
| 147 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:57` |
| 148 | 🟢 | Typo | Typo: 'Oder' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:69` |
| 149 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:69` |
| 150 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:80` |
| 151 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:86` |
| 152 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:96` |
| 153 | 🟢 | Typo | Typo: 'Funktion' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:96` |
| 154 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:96` |
| 155 | 🟢 | Typo | Typo: 'startet' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:106` |
| 156 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:106` |
| 157 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:106` |
| 158 | 🟢 | Typo | Typo: 'deine' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:106` |
| 159 | 🟢 | Typo | Typo: 'ans' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:106` |
| 160 | 🟢 | Typo | Typo: 're-usable' | `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:1093` |
| 161 | 🟢 | Typo | Typo: 'childs' | `docs\_locale\fr\LC_MESSAGES\api.po:622` |
| 162 | 🟢 | Typo | Typo: 'accpets' | `docs\_locale\fr\LC_MESSAGES\changelog.po:498` |
| 163 | 🟢 | Typo | Typo: 'Whats' | `docs\_locale\fr\LC_MESSAGES\changelog.po:521` |
| 164 | 🟢 | Typo | Typo: 'modue' | `docs\_locale\fr\LC_MESSAGES\configuration.po:226` |
| 165 | 🟢 | Typo | Typo: 'ans' | `docs\_locale\fr\LC_MESSAGES\contact.po:39` |
| 166 | 🟢 | Typo | Typo: 'langage' | `docs\_locale\fr\LC_MESSAGES\contact.po:39` |
| 167 | 🟢 | Typo | Typo: 'projet' | `docs\_locale\fr\LC_MESSAGES\contact.po:50` |
| 168 | 🟢 | Typo | Typo: 'projet' | `docs\_locale\fr\LC_MESSAGES\contact.po:50` |
| 169 | 🟢 | Typo | Typo: 'projet' | `docs\_locale\fr\LC_MESSAGES\contact.po:50` |
| 170 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\fr\LC_MESSAGES\contact.po:64` |
| 171 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\fr\LC_MESSAGES\contact.po:66` |
| 172 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\fr\LC_MESSAGES\contact.po:66` |
| 173 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\fr\LC_MESSAGES\contact.po:68` |
| 174 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\fr\LC_MESSAGES\contact.po:68` |
| 175 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\fr\LC_MESSAGES\contact.po:68` |
| 176 | 🟢 | Typo | Typo: 'Thats' | `docs\_locale\fr\LC_MESSAGES\development.po:232` |
| 177 | 🟢 | Typo | Typo: 'applyed' | `docs\_locale\fr\LC_MESSAGES\development.po:285` |
| 178 | 🟢 | Typo | Typo: 'Exemple' | `docs\_locale\fr\LC_MESSAGES\index.po:58` |
| 179 | 🟢 | Typo | Typo: 'informations' | `docs\_locale\fr\LC_MESSAGES\plugindev.po:212` |
| 180 | 🟢 | Typo | Typo: 'infastructure' | `docs\_locale\fr\LC_MESSAGES\recipes.po:291` |
| 181 | 🟢 | Typo | Typo: 're-usable' | `docs\_locale\fr\LC_MESSAGES\tutorial.po:1091` |
| 182 | 🟢 | Typo | Typo: 'childs' | `docs\_locale\ja_JP\LC_MESSAGES\api.po:622` |
| 183 | 🟢 | Typo | Typo: 'accpets' | `docs\_locale\ja_JP\LC_MESSAGES\changelog.po:498` |
| 184 | 🟢 | Typo | Typo: 'Whats' | `docs\_locale\ja_JP\LC_MESSAGES\changelog.po:521` |
| 185 | 🟢 | Typo | Typo: 'modue' | `docs\_locale\ja_JP\LC_MESSAGES\configuration.po:226` |
| 186 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\ja_JP\LC_MESSAGES\contact.po:63` |
| 187 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\ja_JP\LC_MESSAGES\contact.po:65` |
| 188 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\ja_JP\LC_MESSAGES\contact.po:65` |
| 189 | 🟢 | Typo | Typo: 'Thats' | `docs\_locale\ja_JP\LC_MESSAGES\development.po:232` |
| 190 | 🟢 | Typo | Typo: 'applyed' | `docs\_locale\ja_JP\LC_MESSAGES\development.po:285` |
| 191 | 🟢 | Typo | Typo: 'informations' | `docs\_locale\ja_JP\LC_MESSAGES\plugindev.po:212` |
| 192 | 🟢 | Typo | Typo: 'infastructure' | `docs\_locale\ja_JP\LC_MESSAGES\recipes.po:291` |
| 193 | 🟢 | Typo | Typo: 're-usable' | `docs\_locale\ja_JP\LC_MESSAGES\tutorial.po:1092` |
| 194 | 🟢 | Typo | Typo: 'childs' | `docs\_locale\pt_BR\LC_MESSAGES\api.po:624` |
| 195 | 🟢 | Typo | Typo: 'accpets' | `docs\_locale\pt_BR\LC_MESSAGES\changelog.po:498` |
| 196 | 🟢 | Typo | Typo: 'Whats' | `docs\_locale\pt_BR\LC_MESSAGES\changelog.po:521` |
| 197 | 🟢 | Typo | Typo: 'modue' | `docs\_locale\pt_BR\LC_MESSAGES\configuration.po:226` |
| 198 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\pt_BR\LC_MESSAGES\contact.po:63` |
| 199 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\pt_BR\LC_MESSAGES\contact.po:65` |
| 200 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\pt_BR\LC_MESSAGES\contact.po:65` |
| 201 | 🟢 | Typo | Typo: 'Thats' | `docs\_locale\pt_BR\LC_MESSAGES\development.po:232` |
| 202 | 🟢 | Typo | Typo: 'applyed' | `docs\_locale\pt_BR\LC_MESSAGES\development.po:285` |
| 203 | 🟢 | Typo | Typo: 'leve' | `docs\_locale\pt_BR\LC_MESSAGES\index.po:33` |
| 204 | 🟢 | Typo | Typo: 'informations' | `docs\_locale\pt_BR\LC_MESSAGES\plugindev.po:212` |
| 205 | 🟢 | Typo | Typo: 'infastructure' | `docs\_locale\pt_BR\LC_MESSAGES\recipes.po:291` |
| 206 | 🟢 | Typo | Typo: 'ser' | `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:37` |
| 207 | 🟢 | Typo | Typo: 'ser' | `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:37` |
| 208 | 🟢 | Typo | Typo: 'vai' | `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:57` |
| 209 | 🟢 | Typo | Typo: 'te' | `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:57` |
| 210 | 🟢 | Typo | Typo: 'prefere' | `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:57` |
| 211 | 🟢 | Typo | Typo: 'ser' | `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:57` |
| 212 | 🟢 | Typo | Typo: 'vai' | `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:86` |
| 213 | 🟢 | Typo | Typo: 're-usable' | `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:1093` |
| 214 | 🟢 | Typo | Typo: 'returend' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\api.po:400` |
| 215 | 🟢 | Typo | Typo: 'accpets' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\changelog.po:239` |
| 216 | 🟢 | Typo | Typo: 'Whats' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\changelog.po:262` |
| 217 | 🟢 | Typo | Typo: 'Autor' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\contact.po:19` |
| 218 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\contact.po:57` |
| 219 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\contact.po:59` |
| 220 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\contact.po:59` |
| 221 | 🟢 | Typo | Typo: 'Thats' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\development.po:231` |
| 222 | 🟢 | Typo | Typo: 'applyed' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\development.po:284` |
| 223 | 🟢 | Typo | Typo: 'informations' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\plugindev.po:206` |
| 224 | 🟢 | Typo | Typo: 'virtaully' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\plugindev.po:341` |
| 225 | 🟢 | Typo | Typo: 'infastructure' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\recipes.po:264` |
| 226 | 🟢 | Typo | Typo: 're-usable' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\tutorial.po:1132` |
| 227 | 🟢 | Typo | Typo: 'beeing' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\tutorial.po:1284` |
| 228 | 🟢 | Typo | Typo: 'progess' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\tutorial_app.po:20` |
| 229 | 🟢 | Typo | Typo: 'databse' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\tutorial_app.po:40` |
| 230 | 🟢 | Typo | Typo: 'adress' | `docs\_locale\pt_BR\LC_MESSAGES\_pot\tutorial_app.po:751` |
| 231 | 🟢 | Typo | Typo: 'childs' | `docs\_locale\ru_RU\LC_MESSAGES\api.po:622` |
| 232 | 🟢 | Typo | Typo: 'accpets' | `docs\_locale\ru_RU\LC_MESSAGES\changelog.po:498` |
| 233 | 🟢 | Typo | Typo: 'Whats' | `docs\_locale\ru_RU\LC_MESSAGES\changelog.po:521` |
| 234 | 🟢 | Typo | Typo: 'modue' | `docs\_locale\ru_RU\LC_MESSAGES\configuration.po:226` |
| 235 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\ru_RU\LC_MESSAGES\contact.po:63` |
| 236 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\ru_RU\LC_MESSAGES\contact.po:65` |
| 237 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\ru_RU\LC_MESSAGES\contact.po:65` |
| 238 | 🟢 | Typo | Typo: 'Thats' | `docs\_locale\ru_RU\LC_MESSAGES\development.po:232` |
| 239 | 🟢 | Typo | Typo: 'applyed' | `docs\_locale\ru_RU\LC_MESSAGES\development.po:285` |
| 240 | 🟢 | Typo | Typo: 'informations' | `docs\_locale\ru_RU\LC_MESSAGES\plugindev.po:212` |
| 241 | 🟢 | Typo | Typo: 'infastructure' | `docs\_locale\ru_RU\LC_MESSAGES\recipes.po:291` |
| 242 | 🟢 | Typo | Typo: 're-usable' | `docs\_locale\ru_RU\LC_MESSAGES\tutorial.po:1092` |
| 243 | 🟢 | Typo | Typo: 'childs' | `docs\_locale\zh_CN\LC_MESSAGES\api.po:623` |
| 244 | 🟢 | Typo | Typo: 'accpets' | `docs\_locale\zh_CN\LC_MESSAGES\changelog.po:498` |
| 245 | 🟢 | Typo | Typo: 'Whats' | `docs\_locale\zh_CN\LC_MESSAGES\changelog.po:521` |
| 246 | 🟢 | Typo | Typo: 'modue' | `docs\_locale\zh_CN\LC_MESSAGES\configuration.po:226` |
| 247 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\zh_CN\LC_MESSAGES\contact.po:63` |
| 248 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\zh_CN\LC_MESSAGES\contact.po:65` |
| 249 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\zh_CN\LC_MESSAGES\contact.po:65` |
| 250 | 🟢 | Typo | Typo: 'Thats' | `docs\_locale\zh_CN\LC_MESSAGES\development.po:232` |
| 251 | 🟢 | Typo | Typo: 'applyed' | `docs\_locale\zh_CN\LC_MESSAGES\development.po:285` |
| 252 | 🟢 | Typo | Typo: 'informations' | `docs\_locale\zh_CN\LC_MESSAGES\plugindev.po:212` |
| 253 | 🟢 | Typo | Typo: 'infastructure' | `docs\_locale\zh_CN\LC_MESSAGES\recipes.po:291` |
| 254 | 🟢 | Typo | Typo: 're-usable' | `docs\_locale\zh_CN\LC_MESSAGES\tutorial.po:1091` |
| 255 | 🟢 | Typo | Typo: 'unistall' | `docs\_locale\zh_CN\LC_MESSAGES\tutorial.po:1173` |
| 256 | 🟢 | Typo | Typo: 'returend' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\api.po:400` |
| 257 | 🟢 | Typo | Typo: 'accpets' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\changelog.po:239` |
| 258 | 🟢 | Typo | Typo: 'Whats' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\changelog.po:262` |
| 259 | 🟢 | Typo | Typo: 'Autor' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\contact.po:19` |
| 260 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\contact.po:57` |
| 261 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\contact.po:59` |
| 262 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\contact.po:59` |
| 263 | 🟢 | Typo | Typo: 'Thats' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\development.po:231` |
| 264 | 🟢 | Typo | Typo: 'applyed' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\development.po:284` |
| 265 | 🟢 | Typo | Typo: 'informations' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\plugindev.po:206` |
| 266 | 🟢 | Typo | Typo: 'virtaully' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\plugindev.po:341` |
| 267 | 🟢 | Typo | Typo: 'infastructure' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\recipes.po:264` |
| 268 | 🟢 | Typo | Typo: 're-usable' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\tutorial.po:1132` |
| 269 | 🟢 | Typo | Typo: 'beeing' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\tutorial.po:1284` |
| 270 | 🟢 | Typo | Typo: 'progess' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\tutorial_app.po:20` |
| 271 | 🟢 | Typo | Typo: 'databse' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\tutorial_app.po:40` |
| 272 | 🟢 | Typo | Typo: 'adress' | `docs\_locale\zh_CN\LC_MESSAGES\_pot\tutorial_app.po:751` |
| 273 | 🟢 | Typo | Typo: 'childs' | `docs\_locale\_pot\api.pot:513` |
| 274 | 🟢 | Typo | Typo: 'accpets' | `docs\_locale\_pot\changelog.pot:372` |
| 275 | 🟢 | Typo | Typo: 'Whats' | `docs\_locale\_pot\changelog.pot:392` |
| 276 | 🟢 | Typo | Typo: 'modue' | `docs\_locale\_pot\configuration.pot:160` |
| 277 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\_pot\contact.pot:48` |
| 278 | 🟢 | Typo | Typo: 'oder' | `docs\_locale\_pot\contact.pot:48` |
| 279 | 🟢 | Typo | Typo: 'ist' | `docs\_locale\_pot\contact.pot:48` |
| 280 | 🟢 | Typo | Typo: 'Thats' | `docs\_locale\_pot\development.pot:156` |
| 281 | 🟢 | Typo | Typo: 'applyed' | `docs\_locale\_pot\development.pot:188` |
| 282 | 🟢 | Typo | Typo: 'informations' | `docs\_locale\_pot\plugindev.pot:132` |
| 283 | 🟢 | Typo | Typo: 'infastructure' | `docs\_locale\_pot\recipes.pot:217` |
| 284 | 🟢 | Typo | Typo: 're-usable' | `docs\_locale\_pot\tutorial.pot:701` |
| 285 | 🟢 | Typo | Typo: 'doen't' | `test\test_config.py:10` |
| 286 | 🟢 | Typo | Typo: 'overlayed' | `test\test_config.py:118` |
| 287 | 🟢 | Typo | Typo: 'overlayed' | `test\test_config.py:152` |
| 288 | 🟢 | Typo | Typo: 'multible' | `test\test_environ.py:321` |
| 289 | 🟢 | Typo | Typo: 'te' | `test\test_environ.py:866` |
| 290 | 🟢 | Typo | Typo: 'te' | `test\test_environ.py:867` |
| 291 | 🟢 | Typo | Typo: 'returs' | `test\test_formsdict.py:9` |
| 292 | 🟢 | Typo | Typo: 'returs' | `test\test_formsdict.py:15` |
| 293 | 🟢 | Typo | Typo: 'clen' | `test\test_multipart.py:21` |
| 294 | 🟢 | Typo | Typo: 'clen' | `test\test_multipart.py:26` |
| 295 | 🟢 | Typo | Typo: 'Te' | `test\test_multipart.py:59` |
| 296 | 🟢 | Typo | Typo: 'Te' | `test\test_multipart.py:60` |
| 297 | 🟢 | Typo | Typo: 'withoud' | `test\test_multipart.py:130` |
| 298 | 🟢 | Typo | Typo: 'clen' | `test\test_multipart.py:703` |
| 299 | 🟢 | Typo | Typo: 'indention' | `test\test_stpl.py:106` |
| 300 | 🟢 | Typo | Typo: 'indention' | `test\test_stpl.py:117` |
| 301 | 🟠 | Secret | Potential Password/Secret | `bottle.py:2894` |
| 302 | 🟠 | Secret | Potential Password/Secret | `bottle.py:3079` |
| 303 | 🟠 | Secret | Potential Password/Secret | `docs\tutorial.rst:246` |
| 304 | 🟠 | Secret | Potential Password/Secret | `docs\tutorial.rst:459` |
| 305 | 🟠 | Secret | Potential Password/Secret | `docs\tutorial.rst:461` |
| 306 | 🟠 | Secret | Potential Password/Secret | `docs\tutorial.rst:468` |
| 307 | 🟠 | Secret | Potential Password/Secret | `docs\tutorial.rst:615` |
| 308 | 🟠 | Secret | Potential Password/Secret | `test\test_securecookies.py:30` |
| 309 | 🟠 | Secret | Potential Password/Secret | `test\test_securecookies.py:33` |
| 310 | 🟠 | Secret | Potential Password/Secret | `test\test_securecookies.py:37` |
| 311 | 🟠 | Secret | Potential Password/Secret | `test\test_securecookies.py:40` |

---

## Detailed Findings

### 🔐 Exposed Secrets & Credentials

*Hardcoded credentials, API keys, or other sensitive data found in source code.*

#### 1. Potential Password/Secret

**Severity:** 🟠 HIGH  
**Detector:** `regex-patterns`

**Evidence:**

- **File:** `bottle.py:2894`
- **Match (redacted):** `toun********lit(`

**Intent:**

The code appears to store a Password/Secret for authentication or API access. This is likely used to connect to an external service.

**Attack Surface:**

- **Entry Point:** Anyone with access to the source code repository
- **Exposure:** The secret value may be in version control history
- **Reach:** If leaked, attackers can use the credential to access external services

**Risk Assessment:**

- **Impact:** Significant - Data breach or service disruption
- **Likelihood:** High - Secrets in code are easily discovered

**Recommended Fix:**

1. **Remove** the hardcoded secret from the source code
2. **Rotate** the exposed credential immediately
3. **Use** environment variables or a secrets manager
4. **Audit** version control history for the exposed value

**Verification:**

- Re-run the security scanner to confirm removal
- Verify the old credential no longer provides access
- Check git history was cleaned if necessary

---

#### 2. Potential Password/Secret

**Severity:** 🟠 HIGH  
**Detector:** `regex-patterns`

**Evidence:**

- **File:** `bottle.py:3079`
- **Match (redacted):** `requ****auth`

**Intent:**

The code appears to store a Password/Secret for authentication or API access. This is likely used to connect to an external service.

**Attack Surface:**

- **Entry Point:** Anyone with access to the source code repository
- **Exposure:** The secret value may be in version control history
- **Reach:** If leaked, attackers can use the credential to access external services

**Risk Assessment:**

- **Impact:** Significant - Data breach or service disruption
- **Likelihood:** High - Secrets in code are easily discovered

**Recommended Fix:**

1. **Remove** the hardcoded secret from the source code
2. **Rotate** the exposed credential immediately
3. **Use** environment variables or a secrets manager
4. **Audit** version control history for the exposed value

**Verification:**

- Re-run the security scanner to confirm removal
- Verify the old credential no longer provides access
- Check git history was cleaned if necessary

---

#### 3. Potential Password/Secret

**Severity:** 🟠 HIGH  
**Detector:** `regex-patterns`

**Evidence:**

- **File:** `docs\tutorial.rst:246`
- **Match (redacted):** `requ********word`

**Intent:**

The code appears to store a Password/Secret for authentication or API access. This is likely used to connect to an external service.

**Attack Surface:**

- **Entry Point:** Anyone with access to the source code repository
- **Exposure:** The secret value may be in version control history
- **Reach:** If leaked, attackers can use the credential to access external services

**Risk Assessment:**

- **Impact:** Significant - Data breach or service disruption
- **Likelihood:** High - Secrets in code are easily discovered

**Recommended Fix:**

1. **Remove** the hardcoded secret from the source code
2. **Rotate** the exposed credential immediately
3. **Use** environment variables or a secrets manager
4. **Audit** version control history for the exposed value

**Verification:**

- Re-run the security scanner to confirm removal
- Verify the old credential no longer provides access
- Check git history was cleaned if necessary

---

#### 4. Potential Password/Secret

**Severity:** 🟠 HIGH  
**Detector:** `regex-patterns`

**Evidence:**

- **File:** `docs\tutorial.rst:459`
- **Match (redacted):** `requ********get(`

**Intent:**

The code appears to store a Password/Secret for authentication or API access. This is likely used to connect to an external service.

**Attack Surface:**

- **Entry Point:** Anyone with access to the source code repository
- **Exposure:** The secret value may be in version control history
- **Reach:** If leaked, attackers can use the credential to access external services

**Risk Assessment:**

- **Impact:** Significant - Data breach or service disruption
- **Likelihood:** High - Secrets in code are easily discovered

**Recommended Fix:**

1. **Remove** the hardcoded secret from the source code
2. **Rotate** the exposed credential immediately
3. **Use** environment variables or a secrets manager
4. **Audit** version control history for the exposed value

**Verification:**

- Re-run the security scanner to confirm removal
- Verify the old credential no longer provides access
- Check git history was cleaned if necessary

---

#### 5. Potential Password/Secret

**Severity:** 🟠 HIGH  
**Detector:** `regex-patterns`

**Evidence:**

- **File:** `docs\tutorial.rst:461`
- **Match (redacted):** `some*******-key`

**Intent:**

The code appears to store a Password/Secret for authentication or API access. This is likely used to connect to an external service.

**Attack Surface:**

- **Entry Point:** Anyone with access to the source code repository
- **Exposure:** The secret value may be in version control history
- **Reach:** If leaked, attackers can use the credential to access external services

**Risk Assessment:**

- **Impact:** Significant - Data breach or service disruption
- **Likelihood:** High - Secrets in code are easily discovered

**Recommended Fix:**

1. **Remove** the hardcoded secret from the source code
2. **Rotate** the exposed credential immediately
3. **Use** environment variables or a secrets manager
4. **Audit** version control history for the exposed value

**Verification:**

- Re-run the security scanner to confirm removal
- Verify the old credential no longer provides access
- Check git history was cleaned if necessary

---

#### 6. Potential Password/Secret

**Severity:** 🟠 HIGH  
**Detector:** `regex-patterns`

**Evidence:**

- **File:** `docs\tutorial.rst:468`
- **Match (redacted):** `some*******-key`

**Intent:**

The code appears to store a Password/Secret for authentication or API access. This is likely used to connect to an external service.

**Attack Surface:**

- **Entry Point:** Anyone with access to the source code repository
- **Exposure:** The secret value may be in version control history
- **Reach:** If leaked, attackers can use the credential to access external services

**Risk Assessment:**

- **Impact:** Significant - Data breach or service disruption
- **Likelihood:** High - Secrets in code are easily discovered

**Recommended Fix:**

1. **Remove** the hardcoded secret from the source code
2. **Rotate** the exposed credential immediately
3. **Use** environment variables or a secrets manager
4. **Audit** version control history for the exposed value

**Verification:**

- Re-run the security scanner to confirm removal
- Verify the old credential no longer provides access
- Check git history was cleaned if necessary

---

#### 7. Potential Password/Secret

**Severity:** 🟠 HIGH  
**Detector:** `regex-patterns`

**Evidence:**

- **File:** `docs\tutorial.rst:615`
- **Match (redacted):** `requ********word`

**Intent:**

The code appears to store a Password/Secret for authentication or API access. This is likely used to connect to an external service.

**Attack Surface:**

- **Entry Point:** Anyone with access to the source code repository
- **Exposure:** The secret value may be in version control history
- **Reach:** If leaked, attackers can use the credential to access external services

**Risk Assessment:**

- **Impact:** Significant - Data breach or service disruption
- **Likelihood:** High - Secrets in code are easily discovered

**Recommended Fix:**

1. **Remove** the hardcoded secret from the source code
2. **Rotate** the exposed credential immediately
3. **Use** environment variables or a secrets manager
4. **Audit** version control history for the exposed value

**Verification:**

- Re-run the security scanner to confirm removal
- Verify the old credential no longer provides access
- Check git history was cleaned if necessary

---

#### 8. Potential Password/Secret

**Severity:** 🟠 HIGH  
**Detector:** `regex-patterns`

**Evidence:**

- **File:** `test\test_securecookies.py:30`
- **Match (redacted):** `self****ret)`

**Intent:**

The code appears to store a Password/Secret for authentication or API access. This is likely used to connect to an external service.

**Attack Surface:**

- **Entry Point:** Anyone with access to the source code repository
- **Exposure:** The secret value may be in version control history
- **Reach:** If leaked, attackers can use the credential to access external services

**Risk Assessment:**

- **Impact:** Significant - Data breach or service disruption
- **Likelihood:** High - Secrets in code are easily discovered

**Recommended Fix:**

1. **Remove** the hardcoded secret from the source code
2. **Rotate** the exposed credential immediately
3. **Use** environment variables or a secrets manager
4. **Audit** version control history for the exposed value

**Verification:**

- Re-run the security scanner to confirm removal
- Verify the old credential no longer provides access
- Check git history was cleaned if necessary

---

#### 9. Potential Password/Secret

**Severity:** 🟠 HIGH  
**Detector:** `regex-patterns`

**Evidence:**

- **File:** `test\test_securecookies.py:33`
- **Match (redacted):** `self****ret)`

**Intent:**

The code appears to store a Password/Secret for authentication or API access. This is likely used to connect to an external service.

**Attack Surface:**

- **Entry Point:** Anyone with access to the source code repository
- **Exposure:** The secret value may be in version control history
- **Reach:** If leaked, attackers can use the credential to access external services

**Risk Assessment:**

- **Impact:** Significant - Data breach or service disruption
- **Likelihood:** High - Secrets in code are easily discovered

**Recommended Fix:**

1. **Remove** the hardcoded secret from the source code
2. **Rotate** the exposed credential immediately
3. **Use** environment variables or a secrets manager
4. **Audit** version control history for the exposed value

**Verification:**

- Re-run the security scanner to confirm removal
- Verify the old credential no longer provides access
- Check git history was cleaned if necessary

---

#### 10. Potential Password/Secret

**Severity:** 🟠 HIGH  
**Detector:** `regex-patterns`

**Evidence:**

- **File:** `test\test_securecookies.py:37`
- **Match (redacted):** `self****ret)`

**Intent:**

The code appears to store a Password/Secret for authentication or API access. This is likely used to connect to an external service.

**Attack Surface:**

- **Entry Point:** Anyone with access to the source code repository
- **Exposure:** The secret value may be in version control history
- **Reach:** If leaked, attackers can use the credential to access external services

**Risk Assessment:**

- **Impact:** Significant - Data breach or service disruption
- **Likelihood:** High - Secrets in code are easily discovered

**Recommended Fix:**

1. **Remove** the hardcoded secret from the source code
2. **Rotate** the exposed credential immediately
3. **Use** environment variables or a secrets manager
4. **Audit** version control history for the exposed value

**Verification:**

- Re-run the security scanner to confirm removal
- Verify the old credential no longer provides access
- Check git history was cleaned if necessary

---

#### 11. Potential Password/Secret

**Severity:** 🟠 HIGH  
**Detector:** `regex-patterns`

**Evidence:**

- **File:** `test\test_securecookies.py:40`
- **Match (redacted):** `self****ret)`

**Intent:**

The code appears to store a Password/Secret for authentication or API access. This is likely used to connect to an external service.

**Attack Surface:**

- **Entry Point:** Anyone with access to the source code repository
- **Exposure:** The secret value may be in version control history
- **Reach:** If leaked, attackers can use the credential to access external services

**Risk Assessment:**

- **Impact:** Significant - Data breach or service disruption
- **Likelihood:** High - Secrets in code are easily discovered

**Recommended Fix:**

1. **Remove** the hardcoded secret from the source code
2. **Rotate** the exposed credential immediately
3. **Use** environment variables or a secrets manager
4. **Audit** version control history for the exposed value

**Verification:**

- Re-run the security scanner to confirm removal
- Verify the old credential no longer provides access
- Check git history was cleaned if necessary

---

### 📝 Typos & Code Quality

*Spelling errors that may indicate code quality issues or cause bugs.*

#### 1. Typo: 'childs'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `bottle.py:752`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `children, child's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 2. Typo: 'build-in'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `bottle.py:2475`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `built-in`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 3. Typo: 'clen'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `bottle.py:2814`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `clean, clan`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 4. Typo: 'clen'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `bottle.py:2820`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `clean, clan`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 5. Typo: 'clen'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `bottle.py:2840`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `clean, clan`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 6. Typo: 'clen'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `bottle.py:2845`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `clean, clan`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 7. Typo: 'cutted'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `bottle.py:3201`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `cutter, gutted, cut`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 8. Typo: 're-use'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `bottle.py:4212`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `reuse`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 9. Typo: 'loosly'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\changelog.rst:8`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `loosely`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 10. Typo: 'Whats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\changelog.rst:211`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `What's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 11. Typo: 'deprectated'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\deployment.rst:77`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `deprecated`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 12. Typo: 'absolut'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\faq.rst:41`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `absolute`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 13. Typo: 'appropiate'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\faq.rst:271`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `appropriate`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 14. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial.rst:156`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 15. Typo: 'absolut'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial.rst:277`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `absolute`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 16. Typo: 'appropiate'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial.rst:659`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `appropriate`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 17. Typo: 'publically'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:33`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `publicly`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 18. Typo: 'validtion'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:33`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `validation`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 19. Typo: 'formated'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:52`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `formatted`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 20. Typo: 'build-in'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:149`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `built-in`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 21. Typo: 'formated'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:200`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `formatted`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 22. Typo: 'build-in'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:238`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `built-in`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 23. Typo: 'couse'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:317`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `course, cause`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 24. Typo: 'similat'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:473`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `similar`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 25. Typo: 'relativ'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:532`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `relative`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 26. Typo: 'build-in'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:551`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `built-in`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 27. Typo: 'modifiying'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:579`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `modifying`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 28. Typo: 'build-in'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:605`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `built-in`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 29. Typo: 'excuted'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:616`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `executed`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 30. Typo: 'build-in'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:621`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `built-in`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 31. Typo: 'build-in'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:623`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `built-in`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 32. Typo: 'build-in'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:627`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `built-in`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 33. Typo: 'utilizin'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\tutorial_app.rst:669`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `utilizing`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 34. Typo: 're-usable'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\plugins\index.rst:13`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `reusable`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 35. Typo: 'Referenz'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\api.po:24`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Reference`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 36. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\api.po:30`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 37. Typo: 'childs'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\api.po:624`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `children, child's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 38. Typo: 'accpets'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\changelog.po:498`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `accepts`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 39. Typo: 'Whats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\changelog.po:521`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `What's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 40. Typo: 'modue'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\configuration.po:226`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `module`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 41. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\contact.po:50`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 42. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\contact.po:64`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 43. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\contact.po:66`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 44. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\contact.po:66`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 45. Typo: 'Dokument'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:30`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Document`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 46. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:30`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 47. Typo: 'Wege'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:40`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Wedge`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 48. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:53`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 49. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:60`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 50. Typo: 'als'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:99`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `also`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 51. Typo: 'Archiv'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:99`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Archive`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 52. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:99`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 53. Typo: 'Paket'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:118`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Packet`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 54. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:128`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 55. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:128`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 56. Typo: 'alle'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:128`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `all, alley`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 57. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:128`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 58. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:140`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 59. Typo: 'deine'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:140`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `define`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 60. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:155`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 61. Typo: 'hart'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:155`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `heart, harm`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 62. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:155`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 63. Typo: 'Applikation'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:167`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Application`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 64. Typo: 'offen'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:178`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `often`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 65. Typo: 'sie'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:178`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `size, sigh, side`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 66. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:186`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 67. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:196`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 68. Typo: 'Alle'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:196`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `All, Alley`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 69. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:211`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 70. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:211`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 71. Typo: 'als'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:211`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `also`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 72. Typo: 'Alle'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:222`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `All, Alley`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 73. Typo: 'sie'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:222`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `size, sigh, side`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 74. Typo: 'Thats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:233`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `That's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 75. Typo: 'branche'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:235`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `branch, branches, branched`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 76. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:235`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 77. Typo: 'Ende'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:235`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `End`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 78. Typo: 'deine'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:267`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `define`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 79. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:267`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 80. Typo: 'deine'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:267`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `define`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 81. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:267`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 82. Typo: 'alle'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:281`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `all, alley`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 83. Typo: 'applyed'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:286`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `applied`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 84. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:288`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 85. Typo: 'deine'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:288`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `define`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 86. Typo: 'sie'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:288`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `size, sigh, side`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 87. Typo: 'als'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:288`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `also`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 88. Typo: 'deine'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:288`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `define`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 89. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:295`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 90. Typo: 'passt'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:295`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `past, passed`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 91. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:306`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 92. Typo: 'manuell'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:306`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `manual`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 93. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:317`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 94. Typo: 'Als'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:325`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Also`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 95. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:325`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 96. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:333`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 97. Typo: 'lokal'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:333`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `local`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 98. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:342`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 99. Typo: 'deine'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:342`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `define`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 100. Typo: 'sie'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:342`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `size, sigh, side`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 101. Typo: 'deine'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:342`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `define`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 102. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:349`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 103. Typo: 'sie'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:361`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `size, sigh, side`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 104. Typo: 'sie'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:361`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `size, sigh, side`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 105. Typo: 'alle'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:367`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `all, alley`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 106. Typo: 'committe'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:367`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `committee`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 107. Typo: 'deine'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:367`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `define`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 108. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:383`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 109. Typo: 'deine'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:383`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `define`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 110. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:383`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 111. Typo: 'alle'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:383`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `all, alley`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 112. Typo: 'committe'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:383`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `committee`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 113. Typo: 'als'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:389`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `also`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 114. Typo: 'deine'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:389`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `define`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 115. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:398`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 116. Typo: 'deine'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:398`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `define`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 117. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:414`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 118. Typo: 'Branche'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:420`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Branch, Branches, Branched`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 119. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:430`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 120. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\development.po:436`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 121. Typo: 'Ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:32`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Is, It, Its, It's, Sit, List`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 122. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:43`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 123. Typo: 'sie'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:43`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `size, sigh, side`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 124. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:43`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 125. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:43`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 126. Typo: 'Probleme'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:47`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Problem`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 127. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:59`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 128. Typo: 'Probleme'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:81`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Problem`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 129. Typo: 'Adresse'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:91`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Address`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 130. Typo: 'lokal'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:91`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `local`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 131. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:91`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 132. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:91`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 133. Typo: 'lokale'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:91`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `locale`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 134. Typo: 'deines'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:91`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `denies, defines, defined`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 135. Typo: 'Proxys'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:91`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Proxies`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 136. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\faq.po:91`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 137. Typo: 'informations'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\plugindev.po:212`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `information`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 138. Typo: 'infastructure'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\recipes.po:291`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `infrastructure`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 139. Typo: 'Ende'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:37`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `End`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 140. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:37`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 141. Typo: 'als'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:37`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `also`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 142. Typo: 'Referenz'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:37`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Reference`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 143. Typo: 'Sie'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:37`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Size, Sigh, Side`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 144. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:37`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 145. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:37`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 146. Typo: 'alle'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:57`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `all, alley`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 147. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:57`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 148. Typo: 'Oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:69`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Order, Older, Coder, Odder, Odor, Over, Doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 149. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:69`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 150. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:80`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 151. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:86`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 152. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:96`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 153. Typo: 'Funktion'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:96`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Function`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 154. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:96`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 155. Typo: 'startet'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:106`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `started`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 156. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:106`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 157. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:106`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 158. Typo: 'deine'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:106`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `define`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 159. Typo: 'ans'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:106`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `and`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 160. Typo: 're-usable'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\de_DE\LC_MESSAGES\tutorial.po:1093`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `reusable`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 161. Typo: 'childs'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\api.po:622`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `children, child's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 162. Typo: 'accpets'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\changelog.po:498`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `accepts`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 163. Typo: 'Whats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\changelog.po:521`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `What's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 164. Typo: 'modue'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\configuration.po:226`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `module`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 165. Typo: 'ans'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\contact.po:39`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `and`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 166. Typo: 'langage'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\contact.po:39`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `language`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 167. Typo: 'projet'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\contact.po:50`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `project`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 168. Typo: 'projet'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\contact.po:50`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `project`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 169. Typo: 'projet'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\contact.po:50`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `project`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 170. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\contact.po:64`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 171. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\contact.po:66`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 172. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\contact.po:66`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 173. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\contact.po:68`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 174. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\contact.po:68`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 175. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\contact.po:68`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 176. Typo: 'Thats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\development.po:232`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `That's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 177. Typo: 'applyed'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\development.po:285`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `applied`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 178. Typo: 'Exemple'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\index.po:58`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Example`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 179. Typo: 'informations'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\plugindev.po:212`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `information`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 180. Typo: 'infastructure'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\recipes.po:291`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `infrastructure`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 181. Typo: 're-usable'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\fr\LC_MESSAGES\tutorial.po:1091`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `reusable`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 182. Typo: 'childs'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ja_JP\LC_MESSAGES\api.po:622`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `children, child's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 183. Typo: 'accpets'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ja_JP\LC_MESSAGES\changelog.po:498`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `accepts`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 184. Typo: 'Whats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ja_JP\LC_MESSAGES\changelog.po:521`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `What's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 185. Typo: 'modue'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ja_JP\LC_MESSAGES\configuration.po:226`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `module`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 186. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ja_JP\LC_MESSAGES\contact.po:63`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 187. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ja_JP\LC_MESSAGES\contact.po:65`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 188. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ja_JP\LC_MESSAGES\contact.po:65`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 189. Typo: 'Thats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ja_JP\LC_MESSAGES\development.po:232`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `That's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 190. Typo: 'applyed'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ja_JP\LC_MESSAGES\development.po:285`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `applied`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 191. Typo: 'informations'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ja_JP\LC_MESSAGES\plugindev.po:212`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `information`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 192. Typo: 'infastructure'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ja_JP\LC_MESSAGES\recipes.po:291`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `infrastructure`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 193. Typo: 're-usable'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ja_JP\LC_MESSAGES\tutorial.po:1092`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `reusable`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 194. Typo: 'childs'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\api.po:624`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `children, child's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 195. Typo: 'accpets'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\changelog.po:498`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `accepts`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 196. Typo: 'Whats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\changelog.po:521`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `What's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 197. Typo: 'modue'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\configuration.po:226`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `module`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 198. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\contact.po:63`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 199. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\contact.po:65`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 200. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\contact.po:65`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 201. Typo: 'Thats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\development.po:232`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `That's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 202. Typo: 'applyed'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\development.po:285`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `applied`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 203. Typo: 'leve'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\index.po:33`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `level, levee`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 204. Typo: 'informations'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\plugindev.po:212`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `information`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 205. Typo: 'infastructure'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\recipes.po:291`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `infrastructure`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 206. Typo: 'ser'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:37`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `set`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 207. Typo: 'ser'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:37`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `set`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 208. Typo: 'vai'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:57`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `via, vie`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 209. Typo: 'te'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:57`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `the, be, we, to`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 210. Typo: 'prefere'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:57`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `prefer, preferred`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 211. Typo: 'ser'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:57`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `set`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 212. Typo: 'vai'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:86`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `via, vie`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 213. Typo: 're-usable'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\tutorial.po:1093`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `reusable`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 214. Typo: 'returend'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\api.po:400`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `returned`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 215. Typo: 'accpets'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\changelog.po:239`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `accepts`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 216. Typo: 'Whats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\changelog.po:262`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `What's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 217. Typo: 'Autor'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\contact.po:19`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Author`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 218. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\contact.po:57`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 219. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\contact.po:59`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 220. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\contact.po:59`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 221. Typo: 'Thats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\development.po:231`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `That's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 222. Typo: 'applyed'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\development.po:284`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `applied`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 223. Typo: 'informations'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\plugindev.po:206`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `information`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 224. Typo: 'virtaully'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\plugindev.po:341`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `virtually`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 225. Typo: 'infastructure'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\recipes.po:264`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `infrastructure`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 226. Typo: 're-usable'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\tutorial.po:1132`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `reusable`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 227. Typo: 'beeing'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\tutorial.po:1284`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `being, been`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 228. Typo: 'progess'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\tutorial_app.po:20`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `progress`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 229. Typo: 'databse'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\tutorial_app.po:40`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `database`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 230. Typo: 'adress'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\pt_BR\LC_MESSAGES\_pot\tutorial_app.po:751`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `address`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 231. Typo: 'childs'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ru_RU\LC_MESSAGES\api.po:622`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `children, child's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 232. Typo: 'accpets'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ru_RU\LC_MESSAGES\changelog.po:498`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `accepts`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 233. Typo: 'Whats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ru_RU\LC_MESSAGES\changelog.po:521`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `What's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 234. Typo: 'modue'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ru_RU\LC_MESSAGES\configuration.po:226`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `module`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 235. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ru_RU\LC_MESSAGES\contact.po:63`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 236. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ru_RU\LC_MESSAGES\contact.po:65`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 237. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ru_RU\LC_MESSAGES\contact.po:65`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 238. Typo: 'Thats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ru_RU\LC_MESSAGES\development.po:232`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `That's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 239. Typo: 'applyed'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ru_RU\LC_MESSAGES\development.po:285`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `applied`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 240. Typo: 'informations'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ru_RU\LC_MESSAGES\plugindev.po:212`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `information`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 241. Typo: 'infastructure'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ru_RU\LC_MESSAGES\recipes.po:291`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `infrastructure`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 242. Typo: 're-usable'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\ru_RU\LC_MESSAGES\tutorial.po:1092`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `reusable`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 243. Typo: 'childs'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\api.po:623`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `children, child's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 244. Typo: 'accpets'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\changelog.po:498`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `accepts`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 245. Typo: 'Whats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\changelog.po:521`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `What's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 246. Typo: 'modue'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\configuration.po:226`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `module`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 247. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\contact.po:63`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 248. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\contact.po:65`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 249. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\contact.po:65`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 250. Typo: 'Thats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\development.po:232`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `That's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 251. Typo: 'applyed'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\development.po:285`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `applied`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 252. Typo: 'informations'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\plugindev.po:212`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `information`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 253. Typo: 'infastructure'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\recipes.po:291`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `infrastructure`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 254. Typo: 're-usable'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\tutorial.po:1091`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `reusable`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 255. Typo: 'unistall'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\tutorial.po:1173`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `uninstall`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 256. Typo: 'returend'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\api.po:400`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `returned`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 257. Typo: 'accpets'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\changelog.po:239`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `accepts`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 258. Typo: 'Whats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\changelog.po:262`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `What's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 259. Typo: 'Autor'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\contact.po:19`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `Author`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 260. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\contact.po:57`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 261. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\contact.po:59`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 262. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\contact.po:59`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 263. Typo: 'Thats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\development.po:231`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `That's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 264. Typo: 'applyed'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\development.po:284`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `applied`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 265. Typo: 'informations'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\plugindev.po:206`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `information`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 266. Typo: 'virtaully'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\plugindev.po:341`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `virtually`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 267. Typo: 'infastructure'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\recipes.po:264`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `infrastructure`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 268. Typo: 're-usable'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\tutorial.po:1132`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `reusable`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 269. Typo: 'beeing'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\tutorial.po:1284`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `being, been`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 270. Typo: 'progess'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\tutorial_app.po:20`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `progress`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 271. Typo: 'databse'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\tutorial_app.po:40`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `database`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 272. Typo: 'adress'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\zh_CN\LC_MESSAGES\_pot\tutorial_app.po:751`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `address`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 273. Typo: 'childs'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\_pot\api.pot:513`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `children, child's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 274. Typo: 'accpets'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\_pot\changelog.pot:372`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `accepts`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 275. Typo: 'Whats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\_pot\changelog.pot:392`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `What's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 276. Typo: 'modue'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\_pot\configuration.pot:160`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `module`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 277. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\_pot\contact.pot:48`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 278. Typo: 'oder'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\_pot\contact.pot:48`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `order, older, coder, odder, odor, over, doer`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 279. Typo: 'ist'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\_pot\contact.pot:48`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `is, it, its, it's, sit, list`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 280. Typo: 'Thats'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\_pot\development.pot:156`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `That's`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 281. Typo: 'applyed'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\_pot\development.pot:188`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `applied`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 282. Typo: 'informations'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\_pot\plugindev.pot:132`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `information`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 283. Typo: 'infastructure'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\_pot\recipes.pot:217`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `infrastructure`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 284. Typo: 're-usable'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `docs\_locale\_pot\tutorial.pot:701`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `reusable`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 285. Typo: 'doen't'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_config.py:10`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `doesn't`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 286. Typo: 'overlayed'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_config.py:118`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `overlaid`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 287. Typo: 'overlayed'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_config.py:152`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `overlaid`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 288. Typo: 'multible'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_environ.py:321`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `multiple`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 289. Typo: 'te'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_environ.py:866`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `the, be, we, to`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 290. Typo: 'te'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_environ.py:867`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `the, be, we, to`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 291. Typo: 'returs'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_formsdict.py:9`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `returns`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 292. Typo: 'returs'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_formsdict.py:15`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `returns`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 293. Typo: 'clen'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_multipart.py:21`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `clean, clan`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 294. Typo: 'clen'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_multipart.py:26`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `clean, clan`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 295. Typo: 'Te'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_multipart.py:59`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `The, Be, We, To`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 296. Typo: 'Te'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_multipart.py:60`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `The, Be, We, To`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 297. Typo: 'withoud'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_multipart.py:130`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `without`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 298. Typo: 'clen'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_multipart.py:703`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `clean, clan`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 299. Typo: 'indention'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_stpl.py:106`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `indentation`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

#### 300. Typo: 'indention'

**Severity:** 🟢 LOW  
**Detector:** `codespell`

**Evidence:**

- **File:** `test\test_stpl.py:117`

**Intent:**

A spelling error was detected in the code. This may be in comments, strings, or identifiers.

**Attack Surface:**

- **Entry Point:** N/A (code quality issue)
- **Exposure:** May cause confusion or subtle bugs
- **Reach:** Limited security impact, mainly affects maintainability

**Risk Assessment:**

- **Impact:** Minimal - Code quality or minor information disclosure
- **Likelihood:** Low - Unlikely to cause security issues

**Recommended Fix:**

Replace with the correct spelling: `indentation`

**Verification:**

- Run codespell or similar tool to verify fix
- Ensure no new typos were introduced

---

## General Recommendations

### Immediate Actions

1. **Rotate all exposed secrets** - Assume they are compromised

### Preventive Measures

- **Pre-commit hooks**: Use gitleaks or similar to prevent secret commits
- **CI/CD scanning**: Integrate security scanning into the build pipeline
- **Dependency monitoring**: Use Dependabot or Snyk for continuous monitoring
- **Code review**: Include security review in the PR process
- **Developer training**: Educate team on secure coding practices

---

## About This Report

This security report was generated by the **Vulnwright Scanner** developed as part of the MIT Blended AI+X Program (Track 3).

### Limitations

- This is a **static analysis** tool and may produce false positives
- Not all vulnerabilities can be detected through pattern matching
- Human review is essential for accurate risk assessment
- This tool does **not** exploit or test vulnerabilities

### Responsible Disclosure

If this scan revealed potential vulnerabilities in third-party software:

1. Do **NOT** publicly disclose specific vulnerability details
2. Contact the maintainers privately through their security policy
3. Allow reasonable time for patches before any disclosure
4. Follow the project's responsible disclosure guidelines

---

*Report generated on 2026-01-07 07:04:03 UTC*  
*MIT Blended AI+X PBL - Vulnwright*