Python Stress Test Tool
Overview

This repository contains a Python Stress Test Tool, built for developers and system administrators to test the performance and resilience of web applications under extreme load. The tool can simulate high levels of traffic, helping to identify bottlenecks and vulnerabilities in web services.

Designed with flexibility and performance in mind, the tool provides support for:

    Proxy integration for simulating requests from different IP addresses.
    Under Attack Mode (UAM) to bypass anti DDoS Cloudflare mitigation.
    Crawler functionality to navigate and find heavy endpoints automatically.
    Subprocess and Threading to handle high concurrency efficiently, ensuring maximum resource utilization.

Key Features

    Multithreading and Subprocessing: A hybrid approach combining Python's threading and subprocess modules ensures the tool can handle a high number of concurrent requests and operations, teste capacity.

    Proxy Support: Run tests through proxy servers to simulate traffic from different geographic locations or distribute the load across multiple IPs, adding realism to the stress test and spoofing.

    Under Attack Mode (UAM): Bypass Cloudflare Im Under Attack Mode Captcha

    Crawler: Automatically explore and find heavy endpoints of the site navigating through internal links.

    Highly Configurable: Offers a wide range of configurable options, such as request concurrency, timeouts, retry policies, and custom headers, allowing precise control over how the test is executed.

Limitations

    UAM and Proxy Incompatibility: The Under Attack Mode (UAM) feature cannot be used in conjunction with proxy servers due to limitations in handling custom request patterns when proxies are involved. It is recommended to avoid using both features simultaneously.

Installation

    Clone the repository:

    bash

git clone https://github.com/yourusername/python-stress-test-tool.git
cd python-stress-test-tool

Install the required dependencies:

bash

pip install -r requirements.txt
