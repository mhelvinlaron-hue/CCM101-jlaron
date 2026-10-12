# Container Observability

## Nginx Container Setup

I created a Docker container named `client-website` using the Nginx image. Port 8080 on the server was mapped to port 80 inside the container.

```bash
docker run -d --name client-website -p 8080:80 nginx
```

## Website Request Tests

I used `curl` to check whether the web server could respond to requests.

```bash
curl http://localhost:8080
curl http://localhost:8080
curl http://localhost:8080
curl http://localhost:8080/hidden-admin-page
```

The first three commands test the website's main page. The last command requests a page that should not exist and is intended to produce a 404 response.

## Reviewing Access Logs

I displayed the container's recorded activity with:

```bash
docker logs client-website
```

**Recorded HTTP 404 entry:**

[Paste the exact line containing the 404 response from your terminal.]

The access log helps connect a request with the response returned by the server. By examining these records, an administrator can investigate failed requests and distinguish missing pages from successful requests.

## Resource Usage Check

I monitored the running container with:

```bash
docker stats client-website
```

Record the values shown in your own output:

| Metric         | Actual Observation     |
| -------------- | ---------------------- |
| Container      | `client-website`       |
| CPU percentage | [Enter observed value] |
| Memory usage   | [Enter observed value] |
| Memory limit   | [Enter observed value] |

These readings show how much CPU and memory the container was consuming at the time of observation. Rechecking them during application activity can help reveal changes in resource demand.

