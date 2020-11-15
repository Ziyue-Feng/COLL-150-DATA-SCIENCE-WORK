
## Introduction 

Poverty has been one of the biggest threats to civilized human society for hundreds of years. It has brought this world with multiple serious issues and problems like hunger, crimes, underdevelopment and so on. Generally, there are three perspectives in viewing the causes of poverty (Davids and Gouws, 2013). The first theoretical perspective explains poverty in terms of the problems of poor people, such as their lack of abilities, effort or thrift. Individuals themselves are to blame for their own poverty. The second perspective considers poverty as the consequence of unfavorable economic, political, cultural and social forces, such as exploitation by capitalists and lack of social opportunities. The third perspective views poverty as a result of some unforeseen circumstances like illness, bad luck or misfortunes over which poor people have little or no control. (Li, 2016) Just as Amartya Sen has stated in his work Development As Freedom that economic unfreedom (poverty) will breed social unfreedom and meanwhile the latter one can further foster poverty as well. (Sen, A., 1999) If we do not treat poverty as a problem of gigantic proportions and draw up plans for implementations, it will bring out a vicious cycle for the society. Among all the 17 sustainable development goals of the United Nations until 2030, “End poverty in all its forms everywhere” is the first on the list (Tollefson, 2015). The urgency and significance for poverty alleviation and eradication appear without saying.

China becomes under the spotlight when President Xi Jinping has vowed to fulfill the Communists’ original intent, staking his legacy on an ambitious plan to complete the eradication of rural poverty by 2020, ahead of the world target by 10 years. The government has used a variety of approaches to help bring people out of poverty, devoting tens of billions of dollars to the effort and more than $370 billion in loans. Local officials, who are judged partly on their success in improving living standards, are working feverishly to meet Mr. Xi’s deadline.(Xi Jinping Vows No Poverty in China by 2020. That Could Be Hard., 2017) By the end of 2019, based on the data announced by the National Bureau of Statistics of China, there are still 551 millions of people in the rural area who is living under the standard of poverty line. Turning this number into zero becomes this year’s mission impossible for China and the Chinese government. Though the official announcement related to the progress in poverty alleviation is always positive and full of confidence, the huge stress mainly from the explosion of the pandemic make the promised achievement seriously challenging.  

Another huge challenge is the data collection and analysis for poverty assessment. Since China is actually at the very last stage of eradicating absolute poverty, a dynamic dataset becomes urgent and necessary to establish instead of a static one. Data and information related to poverty should be refreshed from time to time in order to maintain the planned process of poverty eradication, which is much more challenging to achieve in the rural area where data collection is inefficient and outdated. Enormous challenges and problems faced in the phase of data collection. Corruption and bureaucracy in these rural areas is one of them. Fake or deceiving local data and information may used for reporting to the central government which strongly tackles the progress and truth of the progress of poverty alleviation in these areas. In addition, it has been brought up by many scholars that a multidimensional assessment system is necessary for covering the real situation about poverty level instead of focusing on income level of GDP per capita. Factors including social and medical security, education are also significant to be counted into poverty assessment as poverty is not only about economic standards but also basic living standards. The necessity to bring new technologies and data science methodologies into the process of poverty assessment is for the dynamic, accuracy, and comprehensiveness of data. 

Based on these considerations, my research will focus on with the help of remote detection technology and data science methodologies to establish a comprehensive poverty assessment system that able to detect accurate and dynamic data in the rural area of China. The central research question will be: To what extent the remote detection and data science methods can improve the comprehensiveness and reliability of poverty assessment and how can a multidimensional assessing system be established in the rural area of China?
 

## DMSP/OLS night-time lights data 

DMSP/OLS night-time data are annual night-time cloud-free image composites of lights of the globe collected by the DMSP/OLS sensors on a low-earth orbiting satellite (at 833 km altitude above earth). DMSP operates satellites in sun-synchronous orbits with night-time overpasses at 8–10 pm local time. With a swath width of 3000 km and 14 orbits per day, each OLS instrument is capable of generating a complete coverage of night-time data in a 24-hour period. The OLS is an oscillating scan radiometer with two spectral bands. The visible band straddles the visible and near-infrared (VNIR) portion of the spectrum (0.5– 0.9 lm) and the thermal band covers the 10.5–12.5 lm spectrum range. At night, the visible band is intensified using a photomultiplier tube (PMT) to permit detection of clouds illuminated by moonlight. The light intensification enables observation of faint sources of VNIR emissions at night on the earth’s surface, including cities, towns, villages, gas flares, heavily lit fishing boats, and fires (Elvidge et al., 1997).  And nighttime images are collected using the VNIR band, which is intensified by a photomultiplier tube to detect radiance emission down to the 5E−1° Watts/cm2/sr range. There are two spatial resolutions of nighttime images: “fine” resolution data have a nominal spatial resolution of 0.56 km, while “smooth” data have a nominal spatial resolution of 2.7 km with 5 × 5 block averaging.
The version 4 DMSP/OLS night-time image products from 2007 to 2009 (30 arc seconds spatial resolution), released by NOAA-NGDC in 2010 at http:// www.ngdc.noaa.gov/dmsp/ downloadV4composites.html, were used for this study. The data is derived by multiplying the average visible band digital number (DN) of cloud-free light detections with the percent frequency of light detection. The inclusion of the percent frequency of detection term normalizes the resulting digital values for variations in the persistence of lighting. (Wang, 2012)





Each pixel in the imageries has a DN value ranging from 0 to 63. Higher DN values associate with more intense lights. The regional total luminance of night-time light can be calculated using the follow Equation (Zhao et al., 2011): 


where B is the regional total luminance of night-time light; Bi is the image DN value, ranging from 1 to 63; Ni is the number of pixels that have a DN value of Bi. 
Poverty is caused by comprehensive aspects of the socio- economic situations. Administrative areas can also affect the poverty evaluation results in different regions. As the above total luminance of night-time light can only represent an intuitive impression of socio-economic activities at night for a region, we used an average light index (ALI) that can better represent the average level of different regions in this study, 


where L is the average light index (ALI); B is the regional total luminance of night-time light; N is the sum of the number of all the pixels with DN value ranging from 1 to 63. 



## Quality of Rural Life(QRL) 

Including the above night-time lights data, other databases from electricity uses, greenhouse gas output to beds in local healthcare institutions will be collectively counted and weighted for a comprehensive index to show up the situation more in a life quality basis instead of economic or income basis. Most of these data will be collected either from the data updated by local bureau or from the National yearbook. It is named as Quality of Rural Life (QRL). The final assessment index system as QRL involves five aspects including income and expenditure, living conditions and cultural life, infrastructure, public service and social security, and ecological environment. 
Since the index selected involves many aspects, and most of them have complex relationships. Considering the characteristics of the index, the coefficient of variation method is used to determine the weight. This method can identify the importance of the index according to its own differences. The greater the difference, the greater the importance. (Ma, 2019)

where QRL is the quality of rural life; Bu is the value of the uth Item; Wu is the weight of the uth Item; Zi is the standardized value of the ith index; Wi is the weight of the ith index. The greater the value of QRL is, the higher the QRL is. 

## Relative Poverty Index(RPI)

Another more economical dimension for poverty assessment will basically rely on the poverty line and income situation. This research will attempt to measure the level of economic development in a region by measuring the differences between the rural per capita net income/rural per capita GDP/rural per capita fiscal revenue of this region and the corresponding average levels of the province, respectively. On this basis, the relative poverty index (RPI) of a region can be measured. The specific calculations and procedures are as follows: 



where RPIr denotes the relative poverty index of the rth county, and the greater the value of RPI, the higher the relative poverty level of this county; PFr denotes the gap ratio of the rural per capita fiscal revenue of the rth county, Fk is a constant (Fk = 3106 Yuan), indicating the rural per capita fiscal revenue of the province, and Fr is the rural per capita fiscal revenue of the rth county; PGr denotes the gap ratio of the rural per capita GDP of the rth county, Gk is a constant (Gk = 27,600 Yuan), indicating the rural per capita GDP of the province, and Gi denotes the rural per capita GDP of the rth county; PIr denotes the gap ratio of the rural per capita net income of the rth county, Ik is a constant (Ik = 9951 Yuan), indicating the rural per capita net income of the province, and Ir denotes the rural per capita net income of the rth county. (Ma, 2019)


## Importance Performance Analysis

On the basis of comprehensive comparison, this study uses the Importance–Performance Analysis (IPA) method to carry out the correlation analysis between the two, and identifies the poverty-stricken areas according to the IPA analysis chart. IPA was first proposed by Martilla and James in 1977 (Sun,2015). The basic idea is that a customer′s satisfaction with a product (or service) is determined by the importance that he or she attaches to its attributes and his or her judgment of attribute performance. IPA was first used in the marketing industry to evaluate corporate brands, products and services. Due to its simple operation, IPA has currently been widely used in various fields. The analysis results are often represented as IPA charts. An IPA chart is usually divided into four areas: high-high area (the first quadrant), high-low area (the second quadrant), low-low area (the third quadrant) and low-high area (the fourth quadrant). Generally, if the characteristic of the data of a region is located in the high RPI-low QRL area, it will be identified as a real poverty region. (Ma, 2019)




























#### Reference

##### Tollefson, J., 2015. UN approves global to-do list for next 15 years. Nature, 525(7570), pp.434-435.
##### Nytimes.com. 2020. Xi Jinping Vows No Poverty In China By 2020. That Could Be Hard. (Published 2017). [online] Available at: https://www.nytimes.com/2017/10/31/world/asia/xi-jinping-poverty-china.html
##### Elvidge, C.D., Baugh, K.E., Kihn, E.A., et al. Mapping city lights with nighttime data from the DMSP Operational Linescan System. Pho- togram. Eng. Remote Sensing 63 (6), 727–734, 1997 
##### Li, Yuheng et al. “Realizing Targeted Poverty Alleviation In China”. China Agricultural Economic Review, vol 8, no. 3, 2016, pp. 443-454. Emerald, `doi:10.1108/caer-11-2015-0157.
##### Shek, D.T.L. (2004), “Beliefs about the causes of poverty in parents and adolescents experiencing economic disadvantage in Hong Kong”, Journal of Genetic Psychology, Vol. 165 No. 3, pp. 272-292. 
##### Davids, Y.D. and Gouws, A. (2013), “Monitoring perceptions of the causes of poverty in South Africa”, Social Indicators Research, Vol. 110, pp. 1201-1220. 
##### Sen, A., 1999. Development As Freedom. Oxford: Oxford University Press.
##### Wang, Wen et al. “Poverty Assessment Using DMSP/OLS Night-Time Light Satellite Imagery At A Provincial Scale In China”. Advances In Space Research, vol 49, no. 8, 2012, pp. 1253-1264. Elsevier BV, doi:10.1016/j.asr.2012.01.025.
##### Ma, Libang et al. “Rural Poverty Identification And Comprehensive Poverty Assessment Based On Quality-Of-Life: The Case Of Gansu Province (China)”. Sustainability, vol 11, no. 17, 2019, p. 4547. MDPI AG, doi:10.3390/su11174547.
##### Saixiang Zhong, Peng Hu, Ximing Xue, Shuo Yang, Peijuan Zhu. Multi-factor comprehensive evaluation model based on the selection of objective weight assignment method[J].Acta Geographica Sinica, 2015, 70(12): 2011-2031.
##### Zhao, N., Currit, N., Samson, E. Net primary production and gross domestic product in China derived from satellite imagery. Ecological Economics 70 (5), 921–928, 2011. 
##### Sun, H.W.; Lv, C.H.Y.; Qi, A.G.; Cao, G.H.; Han, C.H.L. Research on the principles of data standardization in comprehensive evaluation. Chin. J. Health Stat. 2015, 32, 342–344. 
