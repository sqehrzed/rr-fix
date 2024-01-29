# rr-fix for admin center DSM

Replenish:
Because the principles of new cpuinfo and old cpuinfo modification are different, conflicts will occur.
If cpuinfo (old) was enabled before the upgrade, you may encounter the problem that the control panel cannot be opened after the upgrade.
Please execute the following command to restore the js of the control panel. After the restoration, the control panel can be opened. After rebooting, the new cpuionfo addons will take effect.
Or force reinstallation, select 'Force re-install DSM' from grub menu.

Пополнить:
Поскольку принципы модификации новой cpuinfo и старой cpuinfo отличаются, могут возникнуть конфликты.
Если до обновления была включена старая версия cpuinfo, то после обновления вы можете столкнуться с проблемой, что панель управления не открывается.
Выполните следующую команду, чтобы восстановить js панели управления. После восстановления панель управления можно открыть. После перезагрузки новые аддоны cpuionfo вступят в силу.
Или выполните принудительную переустановку, выбрав в меню grub пункт 'Force re-install DSM'.

curl -kL https://github.com/sqehrzed/rr-fix/blob/main/admin_center.js.gz -o /usr/syno/synoman/webman/modules/AdminCenter/admin_center.js.gz
cp -f /usr/syno/synoman/webman/modules/AdminCenter/admin_center.js.gz /usr/syno/synoman/webman/modules/AdminCenter/admin_center.js.gz.bak
