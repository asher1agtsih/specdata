pollutantmean <- function(directory, pollutant, id=1:332){
  data_list <- list.files(path = directory, pattern = ".csv") ## this is the 
  ## list of all the specdata files
  x <- numeric() ## assigning an empty numeric vector to x
  for(i in id){
    myspecdata <- read.csv(data_list[i]) ## Begin a 'for' loop to read data from 
    ## specdata files
    x <- c(x, myspecdata[[pollutant]])
  }
  mean(x, na.rm=T)
}
pollutantmean("~/Documents/Directory/specdata/", "sulfate", 1:10)
