# This CSS is dedicated to fixing some of the items that Dark Reader misses in turning into "Dark Mode" or items that are messed up

## Steps to adding this CSS into Dark Reader are:
1. Open Dark Reader
2. Head to More => All Settings => Advanced => Dev tools
3. Select Dynamic Theme Editor 
4. Copy and paste CSS at the end of the file
5. Hit apply 

```css
================================
rcbb.pshe.lsuhsc.edu

#PSTAB a span {
    background: #1e1e1e !important;
    color: #dddddd !important;
    font-weight: bold !important;
}
#PSTAB .selectedtab a span {
    background: #555555 !important;
    color: #ffffff !important;
}
.app_label {
    font-weight: bold;
}
.pt_classic_plus .PSPUSHBUTTONDISABLED.Left {
    background-color: black !important;
    background-image: none !important;
}
td[id^="tdPTS_"]:not(#PSTAB *),
td[onmouseover]:not(#PSTAB *),
tr[onmouseover]:not(#PSTAB *),
td:not(#PSTAB *):hover,
tr:not(#PSTAB *):hover {
    --darkreader-inline-bgcolor: transparent !important;
    --pt-hover-background-color: transparent !important;
    background-color: transparent !important;
    background-image: none !important;
}
td[id^="tdPTS_"]:hover:not(#PSTAB *),
tr[id^="trPTS_"]:hover td:not(#PSTAB *) {
    background-color: #222 !important;
    transition: background-color 0.1s ease-in-out;
}

================================
```
