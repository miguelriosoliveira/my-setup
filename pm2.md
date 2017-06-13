# Add timestamp to logs
`pm2 start app.js --log-date-format "YYYY-MM-DD HH:mm:ss.SSS Z"`  
where `"YYYY-MM-DD HH:mm:ss.SSS Z"` is any [`momentjs`](momentjs.com) valid format.  

Source(s):
- https://stackoverflow.com/questions/21317852/how-to-add-dates-to-pm2-error-logs
- http://pm2.keymetrics.io/docs/usage/log-management/
