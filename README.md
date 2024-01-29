# rr-fix for admin center DSM
curl -kL https://github.com/sqehrzed/rr-fix/blob/main/admin_center.js.gz -o /usr/syno/synoman/webman/modules/AdminCenter/admin_center.js.gz
cp -f /usr/syno/synoman/webman/modules/AdminCenter/admin_center.js.gz /usr/syno/synoman/webman/modules/AdminCenter/admin_center.js.gz.bak
