# Bright Data 的抓取代理

[![促销](https://github.com/bright-cn/Rotating-Residential-Proxies/blob/main/50%25%20off%20promo%20%281%29.png)](https://www.bright.cn/proxy-types) 

## 关于 Bright Data
Bright Data 是屡获殊荣的领先代理服务商，为全球超过 20,000 名客户提供服务。凭借超过 1 亿个代理 IP、业界领先的技术，以及可按任意国家、城市、运营商和 ASN 进行定位的能力，我们的代理服务已成为开发者的首选。

## 住宅代理
使用 Bright Data 的[抓取代理](https://www.bright.cn/solutions/scraping-proxy)，体验顺畅的网页爬虫服务，享受精准定位、卓越稳定性和快速响应。

- **超过 7200 万个住宅 IP**
- **粘性会话和动态轮换会话**
- **99.95% 的成功率**
- **支持 HTTP(S) 和 SOCKS5**
- **地理位置定位（免费）**

## 主要功能
- **全球覆盖**：住宅代理覆盖 [195 个国家/地区](https://www.bright.cn/locations)。
- **高成功率**：让你的抓取项目实现高达 99.95% 的成功率。
- **快速响应**：平均响应时间约为 0.7 秒。
- **合乎道德的来源**：所有代理均在用户明确同意的情况下获取。
- **无限并发会话**：不受限制地扩展你的业务。

## 定价方案
- **按量付费**：$8/GB，无需按月承诺。
- **月度订阅**：
  - **71 GB**：$7/GB，每月 $499。
  - **166 GB**：$6/GB，每月 $999。
  - **399 GB**：$5/GB，每月 $1999。
  - **企业方案**：可为大规模需求提供定制解决方案。

[![促销](https://github.com/bright-cn/Awesome-Web-Scraping/blob/main/Proxies%20and%20scrapers%20GitHub%20bonus%20banner%20CN.png)](https://www.bright.cn/proxy-types) 

## 住宅代理入门
1. **开始免费试用**：无需信用卡。
2. **集成**：使用我们的 API 或控制面板管理 IP 和配置。
3. **支持的语言**：提供 Python、Java、C#、Node.js 和 Shell 快速入门示例。

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

## ISP 代理
使用 Bright Data 庞大的 [ISP 代理网络](https://www.bright.cn/proxy-types/isp-proxies)，通过直接来自 ISP 的 IP 安全、稳定且高速地采集数据。

- **超过 700,000 个 ISP IP**
- **静态住宅 IP**，具备长期稳定性
- **99.9% 的成功率**
- **支持 HTTP(S) 和 SOCKS5**
- **免费国家/地区级定位**

## 主要功能
- **全球覆盖**：访问[多个国家/地区](https://www.bright.cn/locations)的 ISP IP。
- **高成功率**：访问网站的成功率高达 99.9%。
- **快速稳定**：低延迟、可靠运行，网络可用性达 99.99%。
- **独享 IP 访问**：使用专用 IP 获得稳定一致的连接。
- **合乎道德的来源**：所有 ISP 代理均直接从 ISP 获取，并符合 GDPR 和 CCPA 要求。

## 定价方案
- **按量付费**：$8/GB，无需按月承诺。
- **月度订阅 - 共享**：
  - **10 个 IP**：$1.80/IP，每月 $18 + 增值税。
  - **100 个 IP**：$1.45/IP，每月 $145 + 增值税。
  - **500 个 IP**：$1.40/IP，每月 $700 + 增值税。
  - **1,000 个 IP**：$1.30/IP，每月 $1300 + 增值税。
  - **企业方案**：为大规模数据采集需求提供定制解决方案。
 
- **月度订阅 - 专用**：
  - **10 个 IP**：$3.50/IP，每月 $35 + 增值税。
  - **100 个 IP**：$2.75/IP，每月 $275 + 增值税。
  - **500 个 IP**：$2.60/IP，每月 $1300 + 增值税。
  - **1,000 个 IP**：$2.50/IP，每月 $2500 + 增值税。
  - **企业方案**：为大规模数据采集需求提供定制解决方案。
 
- **月度订阅 - 按 GB 付费**：
  - $7/GB，每月 $499 + 增值税。
  - $6/GB，每月 $999 + 增值税。
  - $5/GB，每月 $1999 + 增值税。
  - **企业方案**：为大规模数据采集需求提供定制解决方案。


## ISP 代理入门
1. **开始免费试用**：无需信用卡。
2. **集成**：通过 Bright Data 控制面板或 API 管理 IP 和配置。
3. **支持的语言**：提供 Python、Java、C#、Node.js 和 Shell 快速入门指南。

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

## 数据中心代理
利用 Bright Data 庞大的[数据中心代理网络](https://www.bright.cn/proxy-types/datacenter-proxies)，以无与伦比的规模和速度进行可靠的数据采集与网页爬虫。

- **超过 770,000 个数据中心 IP**
- **提供[共享](https://www.bright.cn/solutions/shared-proxies)和[专用](https://www.bright.cn/solutions/dedicated-proxies) IP 选项**
- **平均响应时间约 0.24 秒**
- **支持 HTTP(S) 和 [SOCKS5](https://www.bright.cn/solutions/socks5-proxies)**
- **免费国家/地区级定位**

## 主要功能
- **全球覆盖**：访问 [98 个国家/地区](https://www.bright.cn/locations)的数据中心 IP。
- **高成功率**：抓取任务的成功率高达 99.9%。
- **快速可靠**：网络正常运行时间达 99.99%，连接速度快。
- **可定制选项**：根据你的需求选择共享或专用 IP。
- **无限扩展**：不受限制地支持并发会话。

## 定价方案
- **按量付费**：$0.6/GB，无需按月承诺。
- **月度订阅 - 共享**：
  - **10 个 IP**：$1.40/IP，每月 $14 + 增值税。
  - **100 个 IP**：$1.00/IP，每月 $100 + 增值税。
  - **500 个 IP**：$0.95/IP，每月 $475 + 增值税。
  - **1,000 个 IP**：$0.90/IP，每月 $900 + 增值税。
  - **企业方案**：为大规模数据采集提供定制解决方案。

- **月度订阅 - 专用**：
  - **10 个 IP**：$2.20/IP，每月 $22 + 增值税。
  - **100 个 IP**：$1.70/IP，每月 $170 + 增值税。
  - **500 个 IP**：$1.50/IP，每月 $750 + 增值税。
  - **1,000 个 IP**：$1.30/IP，每月 $1300 + 增值税。
  - **企业方案**：为大规模数据采集提供定制解决方案。


- **月度订阅 - 按 GB 付费**：
  - $0.51/GB，每月 $499 + 增值税。
  - $0.45/GB，每月 $999 + 增值税。
  - $0.42/GB，每月 $1999 + 增值税。
  - **企业方案**：为大规模数据采集提供定制解决方案。

立即注册，首次充值可获得 1:1 等额赠送，最高 $500！

## 数据中心代理入门
1. **开始免费试用**：无需信用卡。
2. **集成**：使用 API 或 Bright Data 控制面板管理 IP 和配置。
3. **支持的语言**：提供 Python、Java、C#、Node.js 和 Shell 快速入门指南。

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
### 立即加入 [Bright Data](https://www.bright.cn/)，了解我们为何能成为行业领导者。 
