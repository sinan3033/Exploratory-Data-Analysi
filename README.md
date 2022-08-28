# Exploratory-Data-Analysi

a@ -0,0 +1,26 aQ
+
## Read in the data
+
data <- read. table ("Exploratory Data Analysis Quiz Data/household_power_consumption.txt"
                       sep = ';, header = T)
+
## Change Date column class to Date
data$Date <- as.Date (data$Date, "d/°m/gY")
+ 
## Isolate the data for the required dates
+
data2 <- data[data$Date == as.Date("01/02/2007", "d/9m/Y") | data$Date == as.Date("02/02/2007", "d/9m/gy'), 1
+ 
## Create a png file for the plot
+ 
png(file = "ExData_Plottingl/plot1.png", width = 480, height = 480)
+
## Create the histogram
+
hist(as.numeric (data2$Global_active_power), breaks = 12,
col = "red", main = "Global Active Power"
xlab = "Global Active Power (kilowatts)")
+
## Close the PNG device
+
dev.off() <img width="482" alt="Ekran Resmi 2022-08-28 12 49 42" src="https://user-images.githubusercontent.com/112256749/187067990-494853b7-8843-4877-975d-f07c1922a6fd.png">

