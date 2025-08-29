# bulk-unzipper
zip-batch-extractor

Get-ChildItem *.zip | ForEach-Object { Expand-Archive -Path $_.FullName -DestinationPath ($_.BaseName) -Force }


powershell -command "Get-ChildItem *.zip | ForEach-Object { Expand-Archive -Path $_.FullName -DestinationPath ($_.BaseName) -Force }"



If your folder has

data1.zip
data2.zip


after running the command, you’ll get:

data1\   (unzipped content)
data2\   (unzipped content)
