# Bright Data 的爬虫代理

[![Promo](https://github.com/bright-cn/Rotating-Residential-Proxies/raw/main/50%25%20off%20promo%20(1).png)](https://www.bright.cn/proxy-types)

## 关于 Bright Data
Bright Data 是一家屡获殊荣的领先代理提供商，服务全球超过 20,000 名客户。凭借超过 1 亿个代理 IP、顶尖的技术，以及对任意国家、城市、运营商和 ASN 的精准定位能力，使得我们的代理服务成为开发者的首选。

## 住宅代理
体验 Bright Data 的[住宅代理](https://www.bright.cn/solutions/scraping-proxy)带来的无缝数据抓取能力，精准定位、稳定性和快速响应是我们的核心优势。

- **72M+ 住宅 IP**
- **支持长效会话和轮换会话**
- **99.95% 的成功率**
- **支持 HTTP(S) & SOCKS5**
- **免费地理位置定位**

## 主要特点
- **全球覆盖**：在[195 个国家](https://www.bright.cn/locations)拥有住宅代理网络。
- **高成功率**：抓取项目可达 99.95% 的成功率。
- **快速响应**：平均响应时间约 0.7 秒。
- **道德获取**：所有代理均在获得用户明确同意后提供。
- **无限并发会话**：无使用限制地扩展业务规模。

## 价格方案
- **按量付费**：8.4 美元/GB，无需月度承诺。
- **月度订阅**：
    - **69 GB**：7.14 美元/GB，499 美元/月。
    - **158 GB**：6.3 美元/GB，999 美元/月。
    - **339 GB**：5.88 美元/GB，1999 美元/月。
    - **企业方案**：可为大规模需求提供定制化解决方案。

[![Promo](https://github.com/bright-cn/LinkedIn-Scraper/blob/main/Proxies%20and%20scrapers%20GitHub%20bonus%20banner.png)](https://www.bright.cn/proxy-types)

## 开始使用住宅代理
1. **免费试用**：无需信用卡。
2. **集成**：使用我们的 API 或控制面板来管理 IP 和配置。
3. **支持的语言**：提供 Python、Java、C#、Node.js 和 Shell 的快速入门示例。

## 代码示例

### Python

```python
import sys

# Replace '[your customerID]', 'residential', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335',
             'https': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335',
             'https': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 33335);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-residential", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:33335");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-residential", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335',
})
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:33335 --proxy-user brd-customer-[your customerID]-zone-residential:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

---

## 移动代理
使用 Bright Data 的[移动代理网络](https://www.bright.cn/proxy-types/mobile-proxies)，连接真实的移动设备 IP，涵盖全球数百万个 3G、4G 和 5G IP。

- **7,000,000+ 移动 IP**
- **3G/4G/5G 移动网络 IP**
- **99.99% 在线率，提供 24/7 客服支持**
- **免费地理位置定位**

## 主要特点
- **全球覆盖**：在[195 个国家](https://www.bright.cn/locations)可使用移动 IP。
- **高成功率**：数据采集与测试任务可达 99.9% 的成功率。
- **真实移动连接**：从真实设备与合法网络中获取移动 IP。
- **无限扩容**：支持并发会话与高可用基础设施。
- **运营商级精确定位**：可按运营商进行细分定位，获取更准确的洞察。

## 价格方案
- **按量付费**：8.4 美元/GB，无需月度承诺。
- **月度订阅**：
    - **69 GB**：7.14 美元/GB，499 美元/月 + VAT。
    - **158 GB**：6.3 美元/GB，999 美元/月 + VAT。
    - **339 GB**：5.88 美元/GB，1999 美元/月 + VAT。
    - **企业方案**：可提供定制定价与套餐。

立即注册，您首次充值可享受最高 500 美元的同额赠金！

## 开始使用移动代理
1. **免费试用**：无需信用卡。
2. **集成**：使用 API 或 Bright Data 控制面板来管理 IP 和配置。
3. **支持的语言**：提供 Python、Java、C#、Node.js 和 Shell 的快速入门示例。

## 代码示例

### Python

```python
import sys

# Replace '[your customerID]', 'mobile', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 22225);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-mobile", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:22225");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-mobile", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225',
})
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:22225 --proxy-user brd-customer-[your customerID]-zone-mobile:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

---

## ISP 代理
使用 Bright Data 的[ISP 代理网络](https://www.bright.cn/proxy-types/isp-proxies)，从 ISP 直接获取稳定、快速且安全的 IP，用于数据采集和抓取。

- **700,000+ ISP IP**
- **静态住宅 IP**，长期稳定
- **99.9% 成功率**
- **支持 HTTP(S) & SOCKS5**
- **免费国家级定位**

## 主要特点
- **全球覆盖**：可在[多国](https://www.bright.cn/locations)使用 ISP IP。
- **高成功率**：访问网站成功率高达 99.9%。
- **快速且稳定**：网络延迟低，提供 99.99% 的可用率。
- **专属IP使用**：无需共享 IP，保持连接一致性。
- **道德合规**：所有 ISP 代理直接来自 ISP，遵循 GDPR 和 CCPA 规范。

## 价格方案
- **按量付费**：15 美元/GB（无月度承诺）。
- **月度订阅 - 共享**：
    - **10 IP**：1.80 美元/IP，18 美元/月 + VAT。
    - **100 IP**：1.45 美元/IP，145 美元/月 + VAT。
    - **500 IP**：1.40 美元/IP，700 美元/月 + VAT。
    - **1,000 IP**：1.30 美元/IP，1300 美元/月 + VAT。
    - **企业方案**：适用于大规模数据采集需求的定制化解决方案。

- **月度订阅 - 专属**：
    - **10 IP**：3.50 美元/IP，35 美元/月 + VAT。
    - **100 IP**：2.75 美元/IP，275 美元/月 + VAT。
    - **500 IP**：2.60 美元/IP，1300 美元/月 + VAT。
    - **1,000 IP**：2.50 美元/IP，2500 美元/月 + VAT。
    - **企业方案**：适用于大规模数据采集需求的定制化解决方案。

- **月度订阅 - 按量计费**：
    - 12.75 美元/GB，499 美元/月 + VAT。
    - 11.25 美元/GB，999 美元/月 + VAT。
    - 10.50 美元/GB，1999 美元/月 + VAT。
    - **企业方案**：适用于大规模数据采集需求的定制化解决方案。

## 开始使用 ISP 代理
1. **免费试用**：无需信用卡。
2. **集成**：可通过 Bright Data 控制面板或 API 管理 IP 和配置。
3. **支持的语言**：我们为 Python、Java、C#、Node.js 和 Shell 提供快速入门指导。

## 代码示例

### Python

```python
import sys

# Replace '[your customerID]', 'isp', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 22225);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-isp", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:22225");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-isp", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225',
})
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:22225 --proxy-user brd-customer-[your customerID]-zone-isp:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

---

## 数据中心代理
利用 Bright Data 的[数据中心代理网络](https://www.bright.cn/proxy-types/datacenter-proxies)，规模庞大、速度出众，为可靠的数据采集与网络抓取提供支持。

- **770,000+ 数据中心 IP**
- 提供[共享](https://www.bright.cn/solutions/shared-proxies)和[专属](https://www.bright.cn/solutions/dedicated-proxies) IP 选项
- **平均响应时间约 0.24 秒**
- **支持 HTTP(S) 与 [SOCKS5](https://www.bright.cn/solutions/socks5-proxies)**
- **免费国家级定位**

## 主要特点
- **全球覆盖**：可在[98 个国家](https://www.bright.cn/locations)使用数据中心 IP。
- **高成功率**：抓取任务成功率可达 99.9%。
- **快速且可靠**：99.99% 的网络稳定性与高速连接。
- **可定制选项**：可根据需求选择共享或专属 IP。
- **无限扩容**：支持无限并发会话。

## 价格方案
- **按量付费**：0.6 美元/GB，无需月度承诺。
- **月度订阅 - 共享**：
    - **10 IP**：1.40 美元/IP，14 美元/月 + VAT。
    - **100 IP**：1.00 美元/IP，100 美元/月 + VAT。
    - **500 IP**：0.95 美元/IP，475 美元/月 + VAT。
    - **1,000 IP**：0.90 美元/IP，900 美元/月 + VAT。
    - **企业方案**：可针对大规模数据采集提供定制化解决方案。

- **月度订阅 - 专属**：
    - **10 IP**：2.20 美元/IP，22 美元/月 + VAT。
    - **100 IP**：1.70 美元/IP，170 美元/月 + VAT。
    - **500 IP**：1.50 美元/IP，750 美元/月 + VAT。
    - **1,000 IP**：1.30 美元/IP，1300 美元/月 + VAT。
    - **企业方案**：可针对大规模数据采集提供定制化解决方案。

- **月度订阅 - 按量计费**：
    - 0.51 美元/GB，499 美元/月 + VAT。
    - 0.45 美元/GB，999 美元/月 + VAT。
    - 0.42 美元/GB，1999 美元/月 + VAT。
    - **企业方案**：可针对大规模数据采集提供定制化解决方案。

立即注册并获得首次充值同额赠金，最高可达 500 美元！

## 开始使用数据中心代理
1. **免费试用**：无需信用卡。
2. **集成**：可通过 API 或 Bright Data 控制面板来管理 IP 与配置。
3. **支持的语言**：我们针对 Python、Java、C#、Node.js 和 Shell 提供快速入门示例。

## 代码示例

### Python

```python
import sys

# Replace '[your customerID]', 'datacenter', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 22225);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-datacenter", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:22225");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-datacenter", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225',
    })
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:22225 --proxy-user brd-customer-[your customerID]-zone-residential:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

### 立即加入 [Bright Data](https://www.bright.cn)，体验行业领先的服务。
