# OpenNMS Cheat Sheet

> This document is intended to be used to help diagnose possible OpenNMS issues.

[TOC]

#### Services

Starting the NMS Service:

```bash
systemctl start opennms
```

Restarting the NMS Service:

```bash
systemctl restart opennms
```



#### Opennms Daemons

Restarting a Daemon without restarting the entire Opennms

Restart Provisiond

```bash
/opt/opennms/bin/send-event.pl uei.opennms.org/internal/reloadDaemonConfig --parm 'daemonName Provisiond'
```

Restart Eventd

```bash
/opt/opennms/bin/send-event.pl uei.opennms.org/internal/reloadDaemonConfig --parm 'daemonName Eventd'
```



#### Config Test

OpenNMS configuration tester, this tests the opennms config files for any errors. A good idea to run this before the service is restarted to catch any errors.

```bash
${OPENNMS_HOME}/bin/config-tester -a		
```

For more options run:

```bash
${OPENNMS_HOME}/bin/config-tester -h
```



#### Log files to check

```bash
${OPENNMS_HOME}/logs
```

```bash
journalctl -xe -u opennms
```



#### Config file location

```bash
${OPENNMS_HOME}/etc
```





#### Online resources

[OpenNMS Community](https://opennms.discourse.group/)	[OpenNMS Toolbox](https://toolbox.opennms.eu/)	[OpenNMS Org](https://www.opennms.org/en)



