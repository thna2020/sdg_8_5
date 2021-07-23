# Sustainable Development Goal 8 Target 8.5 in Vietnam
Exploratory Data Analysis of SDG 8 Target 8.5 in Vietnam using SQLite, Pandas, and Matplotlib.

By: Trang Ha Nguyen (Helen), Pomona 2024

## Introduction
The United Nations Sustainable Development Goals (SDGs) are targets for global development adopted in September 2015, set to be achieved by 2030. All countries of the world have agreed to work towards achieving these goals. The 17 Sustainable Development Goals are defined in a list of 169 SDG Targets. Progress towards these Targets is agreed to be tracked by 232 unique Indicators. (United Nations)

## Goal 8: Decent work and economic growth
Over the past 25 years the number of workers living in extreme poverty has declined dramatically, despite the lasting impact of the 2008 economic crisis and global recession. In developing countries, the middle class now makes up more than 34 percent of total employment – a number that has almost tripled between 1991 and 2015.

However, as the global economy continues to recover we are seeing slower growth, widening inequalities, and not enough jobs to keep up with a growing labour force. According to the International Labour Organization, more than 204 million people were unemployed in 2015.

The SDGs promote sustained economic growth, higher levels of productivity and technological innovation. Encouraging entrepreneurship and job creation are key to this, as are effective measures to eradicate forced labour, slavery and human trafficking. With these targets in mind, the goal is to achieve full and productive employment, and decent work, for all women and men by 2030. (United Nations)

### Goal 8
Promote sustained, inclusive and sustainable economic growth, full and productive employment and decent work for all

### Target 8.5
By 2030, achieve full and productive employment and decent work for all women and men, including for young people and persons with disabilities, and equal pay for work of equal value

### Indicator 8.5.1
Average hourly earnings of female and male employees, by occupation, age and persons with disabilities

### Indicator 8.5.2
Unemployment rate, by sex, age and persons with disabilities

## Process
![Process PAA](img/paa.jpg)

Download, Process, and Clean Data
- Download Excel file from UNStats
- View Excel file
- Delete empty, repetitive, and irrelevant columns
- Export to CSV 
- Extract Vietnam’s data from initial dataset with SQL in DB Browser for SQLite

## 8.5.1 Average hourly earnings of female and male employees, by occupation, age and persons with disabilities

### Rationale
Earnings are a key aspect of quality of employment and living conditions. Information on hourly earnings disaggregated by various classifications (sex, age, occupation, disability status) provides some indication of the extent to which pay equality is respected or achieved. (United Nations)

### Limitation & Discrepancy
- Missing 2010 data 
- No data on age and disability status → Can only assess 8.5.1 based on average hourly earnings of female and male employees, by occupation
- Earnings statistics present a number of complications in terms of their international comparability, most of which arise from the variety of possible sources of data. The various sources available -- establishment surveys, household surveys and administrative records -- differ in their methods, objectives and scope, which influences the results obtained. The coverage of the source may vary in terms of the geographical areas covered, the workers covered (for example, part-time workers or informal workers may be excluded) and the establishments covered (for example, establishments below a certain size or of a certain sector may be excluded). In cases where the earnings of workers excluded from the coverage of the source are significantly different than those of workers included, the statistics would not be representative of the country as a whole and would not be strictly comparable to those of countries using a more comprehensive source.
- When using household surveys as a source of earnings statistics, there are a number of issues related to the accuracy of the earnings information reported by the respondents. They may over declare or under declare their earnings for various reasons, or they may report gross or net wages while including or excluding bonuses and benefits, without distinction. This naturally affects the reliability of the results. (United Nations)

### Analysis
Consult Jupyter Notebook file (sdg_8_5.ipynb)

### Assessment - Target 8.5 - Indicator 8.5.1
- Progress? Average Hourly Earnings
- Room for Improvement? Gender Gap in Average Hourly Earnings Across Occupation and Over Time
- Recommendation? Data on Age and Persons with Disabilities

## 8.5.2 Unemployment rate, by sex, age and persons with disabilities

### Rationale
The unemployment rate conveys the percentage of persons in the labour force who are unemployed. The unemployment rate is a useful measure of the underutilization of the labour supply. It reflects the inability of an economy to generate employment for those persons who want to work but are not doing so, even though they are available for employment and actively seeking work. It is thus seen as an indicator of the efficiency and effectiveness of an economy to absorb its labour force and of the performance of the labour market. Short-term time series of the unemployment rate can be used to signal changes in the business cycle; upward movements in the indicator often coincide with recessionary periods or in some cases with the beginning of an expansionary period as persons previously not in the labour market begin to test conditions through an active job search. (United Nations)

### Limitation & Discrepancy
- Missing 2005, 2006, and 2008 data
- No data for Vietnam on disability status → Can only assess 8.5.2 based on unemployment rate, by sex and age
- The significance and meaning of the unemployment rate could be questioned: Even though in most developed countries the unemployment rate is useful as an indicator of labour market performance, and specifically, as a key measure of labour underutilization, in many developing countries, the significance and meaning of the unemployment rate could be questioned. In the absence of unemployment insurance systems or social safety nets, persons of working age must avoid unemployment, resorting to engaging in some form of economic activity, however insignificant or inadequate. Thus, in this context, other measures should supplement the unemployment rate to comprehensively assess labour underutilization. The unemployment rate is dependent on the geographical coverage of the survey since urban and rural areas tend to have significant differences in the incidence of unemployment. It is important to note that unemployment indicators do not convey any information on the characteristics of the unemployed (their education level, ethnic origin, socio-economic background, work experience, duration of unemployment, etc.), which is crucial to cast light on labour market failures. (United Nations)

### Analysis
Consult Jupyter Notebook file (sdg_8_5.ipynb)

### Assessment - Target 8.5 - Indicator 8.5.2
- Progress? Unemployment rate gap by sex
- Room for Improvement? Unemployment rate by age for age group 15-24
- Recommendation? More data on age group 15-24

## Conclusion - Target 8.5 in Vietnam

By 2030, achieve full and productive employment and decent work for all women and men, including for young people and persons with disabilities, and equal pay for work of equal value

- Indicator 8.5.1: Average hourly earnings of female and male employees, by occupation, (age and persons with disabilities - no data)
> Progress? Average Hourly Earnings<br /> 
> Room for Improvement? Gender Gap in Average Hourly Earnings Across Occupation and Over Time<br /> 
> Recommendation? Data on Age and Persons with Disabilities<br /> 

- Indicator 8.5.2: Unemployment rate, by sex, age (and persons with disabilities - no data)
> Progress? Unemployment Rate Gap by Sex<br /> 
> Room for Improvement? Unemployment Rate by Age for Age group 15-24<br /> 
> Recommendation? More Data on Age group 15-24<br /> 

## References
- “Goal 8: Decent Work and Economic Growth: UNDP in Viet Nam.” UNDP, www.vn.undp.org/content/vietnam/en/home/sustainable-development-goals/goal-8-decent-work-and-economic-growth.html. 
- “Những Sự Kiện Kinh Tế Nổi Bật Nhất Trong Năm 2012.” Hanoimoi.com.vn, 1 Jan. 2013, hanoimoi.com.vn/tin-tuc/Kinh-te/571246/nhung-su-kien-kinh-te-noi-bat-nhat-trong-nam-2012.
- “Resolution Concerning Updating the International Standard Classification of Occupations.” International Labour Organization, International Labour Organization, www.ilo.org/public/english/bureau/stat/isco/docs/resol08.pdf. 
- “SDG Indicators - SDG Indicators.” United Nations, United Nations, unstats.un.org/sdgs/metadata/?Text=&amp;Goal=8&amp;Target=8.5. 
- “UNSD - Classification Detail.” United Nations, United Nations, unstats.un.org/unsd/classifications/Family/Detail/1067.
- “Việt Nam 2018 Và 10 Sự Kiện Kinh Tế - Xã Hội Đáng Nhớ.” VnEconomy, 31 Dec. 2018, vneconomy.vn/viet-nam-2018-va-10-su-kien-kinh-te-xa-hoi-dang-nho.htm.
