# Log10x Status Page

Public status page for Log10x services, powered by [Upptime](https://upptime.js.org).

**Live Status:** [status.log10x.com](https://status.log10x.com)

## Monitored Services

| Service       | Description                                |
| ------------- | ------------------------------------------ |
| Console       | Main web application at console.log10x.com |
| API           | Backend API at api.log10x.com              |
| Auth          | Authentication service at auth.log10x.com  |
| Documentation | Product documentation at docs.log10x.com   |
| Grafana       | Dashboards and analytics                   |
| Demo          | Demo environment                           |

## Setup

This repository uses GitHub Actions for automated monitoring:

1. **Uptime checks**: Every 5 minutes
2. **Response time**: Daily
3. **Graphs**: Daily
4. **Static site rebuild**: Daily

### DNS Configuration

Add a CNAME record pointing `status.log10x.com` to `log-10x.github.io`.

### Repository Settings

1. Enable GitHub Pages (Settings > Pages > Source: GitHub Actions)
2. Add custom domain `status.log10x.com`

## For On-Prem Customers

Fork this repository and update `.upptimerc.yml` with your own service URLs:

```yaml
sites:
  - name: Console
    url: https://your-console-url.com
  - name: API
    url: https://your-api-url.com/health
```

## License

MIT
