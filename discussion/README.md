<h1>
  <span class="headline">Identifying Ports and Protocols of Software</span>
  <span class="subhead">Discussion</span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to identify ports and protocols associated with common software applications and explain their purposes in network communication.

## Discussion Introduction

So far, we've learned that network communication relies on ports and protocols. Ports serve as logical channels for software to communicate and exchange data; protocols define the exchange rules.

For this discussion, we'll help you continue familiarizing yourself with this idea by discovering which ports and protocols your favorite applications use.

> ❓ Why do you think some applications need specific ports to function?

## Discovering Ports and Protocols of a System's Applications

Let's get familiar with the tools for this activity.

One of the ways we can do this in **macOS** is to use the `lsof` command (**List Open Files**) to find network connections; here's an example:

```bash
sudo lsof -i -P -n
```

Here's what the appended option flags mean:

- **`-i`**: List network connections only.
- **`-P`**: Show port numbers instead of names.
- **`-n`**: This option avoids DNS lookups for faster results.

>💡 If you're still curious about the `lsof` command, you can access the user manual by running `man lsof`.

On Windows CMD or PowerShell (***be sure to run as Administrator***), we can use `netstat` instead:

```bash
netstat -anb
```

Here's a breakdown of the options we used:

- **`-a`**: Display all active connections.
- **`-P`**: Display addresses and port numbers numerically.
- **`-n`**: Show the executable using the connection.

>💡 If you're still curious about the `netstat` command, you can access the user manual by running `netstat help`.

## Identifying an Application to Analyze

Let's look at the ports and protocols used by the applications on our computers.

1. First, let's choose an application to analyze: a web browser, a messaging app (Slack or Discord), or another application.
2. Next, using the command we reviewed earlier, let's try to find the application's open port(s) and associated protocol (TCP/UDP).

## Guided Discussion Questions

Let's take a moment to reflect on our findings, students should take turns sharing:

1. Which application did you analyze?
2. What ports and protocols are your chosen application using?
3. Are the ports in the well-known range (0-1023), registered range (1024-49151), or dynamic range (49152-65535)?
4. Why do you think this application uses these ports?

## Wrap-up: Independent Exploration

Try identifying ports and protocols for other applications you use frequently (***gaming platforms, video streaming services, or other applications***).

Here are some suggestions:

1. Discord
2. Slack
3. Zoom
4. Chrome, Safari, Firefox, or Edge

Once you're done, you can try going through the questions we discussed earlier on your own to reflect on your findings.
