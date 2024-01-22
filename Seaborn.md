# IN seaborn you need dataframe to work on
## lINE PLOT
import seaborn as sns
### load data
either by
sns.load_dataset()  # or by dataframe  .
sns.lineplot(x=" ",y=" ", hue=" " ,style=" ",data= data,size=   ,palette= " " ,markers=["o" ,">"],dashes=False,legend=True) .
linestyle='--', linewidth=2, marker="^", markerfacecolor='none', markersize=8,markeredgecolor='b'  .

### PASS ANY alphabet in palette you willl get available palette style
### same for legend
### To apply gridd
plt.grid()
plt.title(" ")
plt.fontsize()
plt.show()


## Histogram plot
sns.displot(<datframe column>,bins=[ , , , ,] ,kde=True,rug = True,color= 'k',log_scale=True )
## Barchart
sns.set(style="darkgrid")
sns.barplot(x= " " ,y=" ",data=      ,hue=" ",order=[" " ," ", " "]   ,hue_order=[" "," "] ,ci=1,n_boot=1,orient="v",palette=' ',saturation=   ,errcolor="y",errwidth=  ,capsize=  ,dodge=True,alpha=  )

#for horizontal graph
sns.barplot(x= " " ,y=" ",data=      ,hue=" ",,orient="h" )

#pass order array that you will generate
#pass hue_order array that you will generate
#CI is confidence interval can be 0 to 100


# Scatter plot
m={"Male":"+","Female":"o"}
sns.scatterplot(x= " " ,y=" ",data=      ,hue=" ",style=" ",size=" ",sizes=(100,40),palette=" ",alpha=<0to1> ,markers=m)
# Heatmap (not for string values)
## convert dataframe in 2-d array 
v=sns.heatmap(<dataframe>,vmin=0,vmax=10,cmap="PuOr",annot=True,fmt="s",anot_kws={"fontsize":10,"color:"r"},linewidth=10,linecolor="y",cbar=True,xticklabels=False,yticklabels=False,)
#to give your own input to annot you can pass a array to annot keyword containing the annotations
v.set(xlabel="  ",ylabel= " ")
sns.font_scale=
# Seaborn count plot
#barplot plots mean of category , countplot plots the count in category
sns.countplot(x=" ",data=var,hue="  ",palette="  ",saturation= 0 to 1,)

# Violin plot
### plays similar role as boxplot and whisker plot Shows distribution of quantitative data acrosss several levels of one categorical variablessuch that those distributions can be compared.

sns.violinplot(x=" ",y="  ",data=    ,hue="  ",linewidth=    ,palette="   ",color=" " , saturation = 0to1,order=[" ", " " ],split=True,scale="count"/"area"/"width",inner="quart"/"box"/"quartile"/"point"/"stick"/"None"  )
#you can also plot single violin plot just by giving the x attribute 
#to plot horizontally give x axis data to y and vice versa.

# pair plot
for machine learning algorithm
sns.parplot(<dataframe>,vars=[" " ,"  " ,"  "],hue="  ",hue_order=["  ", "   "],palette="  ",y_vars=["  " ,"  ", " "],kind="reg/scatter/kde/hist",dia_kind="kde/hist",markers=[" ", " "])

# strip plot
vey simple to understand.basically scatter plot that differentiates different categories,good alternative to box/violin plot,

#vars parameter for choosy plotting
sns.strioplot(x=" ", y="  ",data=   ,hue=" ',palette="  ",linewidth=   ,edgecolor=" ",jitter=1,size=  ,marker={"   ": "  ","  ":"  "},alpha=)

# box plot
sns.set(style="whitegrid")
sns.boxplot(x="  ",y="  ",data=    ,hue="  ",color=" ",order=[  " "," ", "  " ],showmeans=True,meanprops={"marker":"  ","markeredgecolor": " "},linewidth=   ,palette="  ",orient=" v"  )


# factor plot
#point plot
sns.factorplot(x= " ",y="  ",data=   ,hue="  ",kind="bar/box/scatter")

# cat plot
same arguments as factorplot
ki nd arguments= point/strip/swarm/box/violin/boxen/bar/count

# styling plot
sns.set_style("    ")
sns.despine() removes right axis line
plt.figure(figsize=( , )
sns.set_context("poster/paper/notebook",font_scale= )

# facet grid
df=sns.load_dataset( )
graph=seaborn.FacetGrid(df, col= "  ",hue="  ")
graph.map(plt.scatter, "  x "  ,"y ").add_legend()
  
