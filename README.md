# AdsListServices

**List of advertisements services**

---

- **Hosts:**
  [View the list](https://raw.githubusercontent.com/MetalistPavlenko/AdsListServices/main/hosts.txt)

- **Domains:**
  [View the list](https://raw.githubusercontent.com/MetalistPavlenko/AdsListServices/main/domains.txt)

---

- **GeoSite for sing-box:**
  [Download database](https://raw.githubusercontent.com/MetalistPavlenko/AdsListServices/main/geosite.srs)

- **GeoSite for xray-core / v2ray-core / mihomo:**
  [Download database](https://raw.githubusercontent.com/MetalistPavlenko/AdsListServices/main/geosite.dat)

---

<details>
<summary style="font-size: 1.1em;"><strong>Apply in RouterOS:</strong></summary>

#### **Importation:**

> **1. Load the `hosts.txt` file into the firmware**

> **2. Change DNS cache size:**
>> ```shell
>> /ip/dns set cache-size=73728
>> ```

> **3. Importing domains:**
>> ```shell
>> /ip/dns/adlist add file=hosts.txt
>> ```

#### **Removal:**

> **1. Removing domains:**
>> ```shell
>> /ip/dns/adlist remove [find file=hosts.txt]
>> ```

> **2. Clearing DNS cache:**
>> ```shell
>> /ip/dns/cache flush
>> ```
</details>