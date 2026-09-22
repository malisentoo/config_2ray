<div align="center">

# 🖤 VPN Configs Hub 🤍

### Конфигурации для обхода блокировок

<img src="https://img.shields.io/badge/VLESS-000000?style=for-the-badge&logo=shadowsocks&logoColor=white" />
<img src="https://img.shields.io/badge/Hysteria2-000000?style=for-the-badge&logo=v2ray&logoColor=white" />
<img src="https://img.shields.io/badge/Trojan-000000?style=for-the-badge&logo=protonvpn&logoColor=white" />
<img src="https://img.shields.io/badge/Shadowsocks-000000?style=for-the-badge&logo=torproject&logoColor=white" />

<img src="https://img.shields.io/badge/License-MIT-white?style=flat-square&labelColor=000000" />
<img src="https://img.shields.io/badge/Status-Active-white?style=flat-square&labelColor=000000" />
<img src="https://img.shields.io/badge/Platform-Cross--Platform-white?style=flat-square&labelColor=000000" />
<img src="https://img.shields.io/github/stars/username/repo?style=flat-square&color=black&labelColor=000000" />

---

**Готовые конфигурации для приложений VPN/прокси-клиентов**
Подходит для обхода интернет-цензуры и сетевых ограничений

[Быстрый старт](#-быстрый-старт) • [Протоколы](#-протоколы) • [Клиенты](#-рекомендуемые-клиенты) • [FAQ](#-faq)

</div>

---

## 📋 Содержание

- [О репозитории](#-о-репозитории)
- [Протоколы](#-протоколы)
- [Быстрый старт](#-быстрый-старт)
- [Рекомендуемые клиенты](#-рекомендуемые-клиенты)
- [Структура репозитория](#-структура-репозитория)
- [Установка Happ](#-установка-happ)
- [FAQ](#-faq)
- [Дисклеймер](#-дисклеймер)

---

## ⚪ О репозитории

Данный репозиторий содержит **готовые конфигурационные файлы** для популярных протоколов обхода блокировок. Конфиги предназначены для личного использования в целях обеспечения свободного и безопасного доступа к интернету.

```
┌─────────────────────────────────────────┐
│  🖤  VLESS + Reality                     │
│  🤍  Hysteria2                           │
│  🖤  Trojan                              │
│  🤍  Shadowsocks (SS)                    │
└─────────────────────────────────────────┘
```

---

## 🔌 Протоколы

<table>
<tr>
<th align="left">Протокол</th>
<th align="left">Особенности</th>
<th align="left">Рекомендуется для</th>
</tr>
<tr>
<td><b>VLESS + Reality</b></td>
<td>Маскировка под TLS-трафик реальных сайтов, высокая скрытность</td>
<td>Строгие DPI-блокировки</td>
</tr>
<tr>
<td><b>Hysteria2</b></td>
<td>Работа поверх QUIC/UDP, высокая скорость, устойчивость к потерям пакетов</td>
<td>Нестабильные сети, видео/стриминг</td>
</tr>
<tr>
<td><b>Trojan</b></td>
<td>Маскируется под обычный HTTPS-трафик</td>
<td>Универсальное использование</td>
</tr>
<tr>
<td><b>Shadowsocks</b></td>
<td>Лёгкий протокол, минимальные задержки</td>
<td>Мобильные сети, экономия батареи</td>
</tr>
</table>

---

## 🚀 Быстрый старт

### 1️⃣ Выберите клиент под вашу платформу

| ОС | Клиент |
|---|---|
| 🖥️ Windows | Happ / v2rayN / NekoRay |
| 🍎 macOS | Happ / V2Box |
| 🐧 Linux | v2rayA / Nekoray |
| 📱 Android | Happ / v2rayNG |
| 📱 iOS | Happ / Shadowrocket / Streisand |

### 2️⃣ Скопируйте ссылку конфига

Конфиги хранятся в формате `vless://`, `hy2://`, `trojan://`, `ss://` — просто скопируйте нужную строку из соответствующего файла в папке `configs/`.

### 3️⃣ Импортируйте в клиент

```
Клиент → Добавить сервер → Импорт из буфера обмена / QR-кода
```

### 4️⃣ Подключитесь и проверьте IP

```bash
curl ifconfig.me
```

---

## 📱 Рекомендуемые клиенты

<div align="center">

| Клиент | Платформы | Поддержка протоколов |
|:---:|:---:|:---:|
| **Happ** | Windows / macOS / iOS / Android | VLESS, Trojan, SS, Hysteria2 |
| **v2rayN** | Windows | VLESS, Trojan, SS |
| **NekoRay** | Windows / Linux | VLESS, Trojan, SS, Hysteria2 |
| **v2rayNG** | Android | VLESS, Trojan, SS, Hysteria2 |
| **Shadowrocket** | iOS | VLESS, Trojan, SS |

</div>

---

## ⚫ Установка Happ

**Happ** — один из самых удобных клиентов с поддержкой всех перечисленных протоколов и простым импортом подписок.

1. Скачайте приложение с официального сайта или магазина приложений вашей платформы
2. Откройте приложение → **Добавить профиль** → **Импорт по ссылке / QR-коду**
3. Вставьте ссылку на подписку или отдельный конфиг
4. Нажмите **Подключиться**

> 💡 Happ поддерживает автоматическое обновление подписок — конфиги обновляются без ручного вмешательства.

---

## 📁 Структура репозитория

```
📦 vpn-configs
├── 📂 configs/
│   ├── 📄 vless.txt
│   ├── 📄 hysteria2.txt
│   ├── 📄 trojan.txt
│   └── 📄 shadowsocks.txt
├── 📂 subscriptions/
│   └── 📄 subscription-link.txt
├── 📂 qr-codes/
│   └── 🖼️ *.png
└── 📄 README.md
```

---

## ❓ FAQ

<details>
<summary><b>Конфиги не подключаются, что делать?</b></summary>
<br>
Проверьте актуальность файла — сервера могут обновляться. Попробуйте другой протокол или клиент.
</details>

<details>
<summary><b>Какой протокол выбрать?</b></summary>
<br>
Для максимальной скрытности — <b>VLESS + Reality</b>. Для скорости и стабильности на плохих сетях — <b>Hysteria2</b>.
</details>

<details>
<summary><b>Как часто обновляются конфиги?</b></summary>
<br>
Следите за датой последнего коммита в репозитории.
</details>

---

## ⚠️ Дисклеймер

Репозиторий создан в информационных и образовательных целях, а также для содействия свободному доступу к информации. Используйте конфигурации в соответствии с законодательством вашей страны. Автор не несёт ответственности за использование материалов третьими лицами.

---

<div align="center">

**🖤🤍 Свобода интернета начинается с одного клика 🤍🖤**

<img src="https://img.shields.io/badge/Made%20with-%E2%9D%A4-black?style=flat-square&labelColor=000000" />

</div>
