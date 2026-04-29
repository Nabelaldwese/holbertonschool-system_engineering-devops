# Web Infrastructure Design

This directory contains answers for the **Web Infrastructure Design** project in the Holberton System Engineering / DevOps track.

## Task 0: Simple Web Stack

File: `0-simple_web_stack`

This task describes a one-server infrastructure hosting `www.foobar.com` with:

- One server (`8.8.8.8`)
- One web server (`Nginx`)
- One application server
- One application code base
- One database (`MySQL`)

It also explains:

- The role of each component
- DNS records used for `www.foobar.com`
- How a user request flows through the stack
- Infrastructure limitations (SPOF, downtime risk, and scaling limits)

## Task 1: Distributed Web Infrastructure

File: `1-distributed_web_infrastructure`

This task describes a three-server distributed infrastructure hosting `www.foobar.com` with:

- One load balancer (`HAproxy`)
- Two application servers (each with `Nginx`, application server, and application files)
- One `MySQL` Primary-Replica setup

It also explains:

- Why each additional element is added
- The `round-robin` distribution algorithm
- `Active-Active` vs `Active-Passive`
- How Primary-Replica replication works
- Remaining limitations (SPOF, no firewall/HTTPS, no monitoring)

## Task 2: Secured and Monitored Web Infrastructure

File: `2-secured_and_monitored_web_infrastructure`

This task describes a secured and monitored three-server infrastructure for `www.foobar.com` with:

- One load balancer (`HAproxy`) with SSL termination
- Three firewalls (one per server)
- Three monitoring agents/clients (one per server)
- Two application servers (`Nginx` + app server + app files)
- One `MySQL` Primary-Replica setup

It also explains:

- Why firewalls, HTTPS, and monitoring are added
- How monitoring data is collected
- How to monitor web server QPS
- Remaining design issues (SSL termination risks, single writable DB node, mixed server roles)

## Task 3: Scale Up

File: `3-scale_up`

This task describes a scaled-up infrastructure for `www.foobar.com` with:

- One additional server
- A second `HAproxy` load balancer clustered with the first
- Split architecture where web, application, and database components are hosted on dedicated servers

It also explains:

- Why each new element is added
- How this design improves availability and scalability
- Why separating service roles improves operations and performance

## Note

Replace the placeholder screenshot links in:

- `0-simple_web_stack`
- `1-distributed_web_infrastructure`
- `2-secured_and_monitored_web_infrastructure`
- `3-scale_up`

with your real diagram URLs (for example, Imgur links) before submission.
