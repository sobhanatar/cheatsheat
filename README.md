# Cheat Sheet

## CURL Commands
- get response time of a url: `curl -o /dev/null -s -w 'Total: %{time_total}s\n' "http://..."`

## CRON Commands
- execute cronjob with different user in a container: `* * * * * sudo docker exec -iu {user name} {service name} bash -c 'php artisan schedule:run' >> /var/log/cron/{service name}.log 2>&1`
