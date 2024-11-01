# Command-Injection

## Planform: rangeforce
## Scenario
As a security specialist, you have just become aware of a widely used website hosted by your company that provides a pinging service. Noticing that the output looks a lot like the output of the ping shell command, you decide to investigate the application for security vulnerabilities.

In this challenge, you will leverage a command injection vulnerability to execute commands on the vulnerable server.

## Learning Objectives
Understand the concept of command injection vulnerabilities.

Gain hands-on experience in exploiting such vulnerabilities in a controlled environment.

Develop skills in using web application testing tools and techniques.

Document the exploitation process for professional portfolio inclusion.

## Steps

**Step 1: Identify the Input Fields**

The application includes fields for:

<img width="287" alt="image" src="https://github.com/user-attachments/assets/3ff72798-af9e-4cc3-aa43-dc1eed01d08d">

**Step 2: Craft the Malicious Input**

To exploit the command injection vulnerability, a payload needs to be crafted. The goal is to inject a command after a valid input.

**Malicious Input:**
127.0.0.1; touch /var/lib/ping-tool/web-app/pwn.txt

## How I think this vulnerability can be prevented:


To prevent command injection vulnerabilities, implement strict input validation and sanitization, ensuring only expected formats are accepted. Utilize secure APIs instead of executing shell commands directly and enforce the principle of least privilege by running applications with minimal permissions. Regular security audits and code reviews can help identify and mitigate vulnerabilities early. Educating developers on secure coding practices further enhances overall security awareness and resilience against such threats.
