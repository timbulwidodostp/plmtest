# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Lagrange FF Multiplier Tests for Panel Models Use plmtest (plm) With (In) R Software
install.packages("plm")
library("plm")
# Estimates Lagrange FF Multiplier Tests for Panel Models Use plmtest (plm) With (In) R Software
plmtest = read.csv("https://raw.githubusercontent.com/timbulwidodostp/plmtest/main/plmtest/plmtest.csv", sep = ";")
plm <- plm(Dependen ~ Independen_1 + Independen_2, data = plmtest, model = "pooling")
plmtest <- plmtest(plm, type = "honda",  effect = "time")
plmtest_2 <- plmtest(plm, type = "bp",  effect = "time")
plmtest_3 <- plmtest(plm, type = "kw",  effect = "time")
plmtest
plmtest_2
plmtest_3
# Lagrange FF Multiplier Tests for Panel Models Use plmtest (plm) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished