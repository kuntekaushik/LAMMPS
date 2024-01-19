# IN seaborn you need dataframe to work on
## lINE PLOT
import seaborn as sns
### load data
either by
sns.load_dataset()  # or by dataframe
sns.lineplot(x=" ",y=" ", hue=" " ,style=" ",data= data,size=   ,palette= " " ,markers=["o" ,">"],dashes=False,legend=True)

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
sns.heatmap(<dataframe>)

