# rain_temp
R Script for extracting rain/precipitation and temperature data using raster and shape files
# This code assumes that you have already downloaded the ncdf (RAIN) files. If not, you can download via ftp:
#ftp://ftp.cpc.ncep.noaa.gov/precip/CPC_UNI_PRCP/
#or manually via your computer browser at https://psl.noaa.gov/data/gridded/data.cpc.globalprecip.html
#For temperature, you can ftp via:
#data_name<-paste0("ftp://ftp.cdc.noaa.gov/Datasets/cpc_global_temp/tmax.",year,".nc") [change the year as appropriate]
#data_name2<-paste0("tmax.",year)
#temp<-GET(data_name,write_disk(paste0("Working Directory/Tmax/",data_name2,".nc"),overwrite=TRUE))
# Read in the shape file. Shape file should be included without .shp extension
#my shape file for zimbabwe is =zwe_admbnda_adm1_zimstat_ocha_20180911

#After extracting the data
#Now you can use R or any other software to clean up the excel file. I use STATA. 
#Geoinpoly function in STATA allows you to map shape files to the coordinates in this file
