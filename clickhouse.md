## find records between dates
```
select ts,topic,is_request,is_response,is_wildcard,value 
    from resolver_log 
where hostname='ns.pci-fs.com' and dateDiff('day',ts,now()) < 30
```