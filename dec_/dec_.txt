# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Performs decomposition of the quantile difference (of y) between two groups (in 2 components) in the common support Use dec_ (decr) With (In) R Software
install.packages("remotes")
remotes::install_github("gibonet/decr")
library("decr")
dec_ = read.csv("https://raw.githubusercontent.com/timbulwidodostp/dec_/main/dec_/dec_.csv",sep = ";")
# Estimation Performs decomposition of the quantile difference (of y) between two groups (in 2 components) in the common support Use dec_ (decr) With (In) R Software
dec_ <- reweight_strata_all2(dec_, treatment = "gender", variables = c("sector", "education"), y = "wage", weights = "sample_weights")
dec_quantile <- dec_quantile(dec_)
dec_ <- dec_(dec_quantile)
dec_
# Performs decomposition of the quantile difference (of y) between two groups (in 2 components) in the common support Use dec_ (decr) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished