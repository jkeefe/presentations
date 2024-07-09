MAPSHAPER:=./node_modules/.bin/mapshaper

initialize:
	-mkdir ./tmp
	-mkdir ./data

download:
	wget --no-check-certificate https://ftp.wpc.ncep.noaa.gov/shapefiles/qpf/5day/QPF120hr_Day1-5_latest.tar -O tmp/latest.tar
	tar --extract --file tmp/latest.tar -C tmp/

rainmap:
	${MAPSHAPER} tmp/95e*.shp \
		-filter "QPF > 1" \
		-classify QPF colors=Purples breaks=1,2,3,5,10 \
		-o format=geojson ./data/latest.json
		