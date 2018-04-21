# B10fip-reliever
#Fielding Independent Pitching by Class (Big Ten Conference) in 2017. Walks and Strikeouts part of the analysis.

library(ggpubr)
library(ggsci)

ggscatter(data = B10fip, x = "so.", y = "fip", label = "Player..", 
          facet.by = "Class", color = "bb.",
          title = "Big 10 Relievers: FIP by Class 2017", 
          xlab = "Strikeouts", ylab = "Fielding Independent Pitching", 
          conf.int = TRUE, add = "reg.line")
