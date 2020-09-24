hello_world

if you want to try, just try it.

Keeling_Data <- read.csv(file = "co2_mm_mlo.csv", header = T)
colnames(Keeling_Data)
head(Keeling_Data)
head(Keeling_Data,3)
tail(Keeling_Data,4)
Keeling_Data$co2
# Min
min(Keeling_Data$co2)
# Max
max(Keeling_Data$co2)
# Range
range(Keeling_Data$co2)
# Mean
mean(Keeling_Data$co2)
# Median
median(Keeling_Data$co2)
# Plot the histogram
hist(Keeling_Data$co2)
# Show quantiles
summary(Keeling_Data$co2)
Keeling_Data$co2[1:10]
Keeling_Data$year[200:210]
plot(Keeling_Data$decimal_date, Keeling_Data$co2)
plot(Keeling_Data$decimal_date, Keeling_Data$co2, ylim=c(300,420), type="l")
Year     <- Keeling_Data$decimal_date
CO2_ppm  <- Keeling_Data$co2 
CO2_ppm[which(CO2_ppm == -99.99)]  <- NA
plot(Year, CO2_ppm, type="l")
mean(CO2_ppm)
mean(CO2_ppm, na.rm=T)
Keeling_Data$co2[1:10] * 1e3
Keeling_Data$month[1:10] + Keeling_Data$co2[1:10]
typeof(Keeling_Data$co2)
typeof(Keeling_Data$month)
typeof(Keeling_Data$quality)
x <- 1 <= 2
typeof(x)
typeof(1+1i)
class(Keeling_Data)
vector_1 <- vector(length = 3)
vector_1
vector_2 <- vector(mode='character', length=3)
vector_2
str(vector_2)
str(Keeling_Data$co2)
vector_3 <- c(1,2,3)
vector_3
vector_4 <- c(1,2,3,"4")
vector_4
vector_5 <- c("a", TRUE)
vector_5
vector_6 <- c(0, TRUE)
vector_6
vector_7 <- c('0','2','4')
vector_7
str(vector_7)
Keeling_Data$quality[1:10]
Keeling_Data$quality <- as.logical(Keeling_Data$quality)
# New data
Keeling_Data$quality[1:10]
length(Keeling_Data$quality)
x <- 1:26
x <- x * 2
names(x) <- LETTERS
x
str(Keeling_Data$month)
Keeling_Data$month <- factor(Keeling_Data$month)
class(Keeling_Data$month)
str(Keeling_Data$month)
typeof(Keeling_Data$month)
list_1 <- list(1, "a", TRUE, 1+4i)
list_1
list_2 <- list(title = "Numbers", numbers = 1:10, data = TRUE )
list_2
typeof(Keeling_Data)
Keeling_Data[,1]
Keeling_Data[,2]
matrix_1 <- matrix(0, ncol=6, nrow=3)
matrix_1
class(matrix_1)
typeof(matrix_1)
str(matrix_1)
dim(matrix_1)
nrow(matrix_1)
ncol(matrix_1)
array_1 <- array(NA, 3)
print(array_1)
array_2 <- array(NA, dim=c(2,3))
print(array_2)
array_3 <- array(NA, dim=c(2,3,3))
print(array_3)
class(array_3)
