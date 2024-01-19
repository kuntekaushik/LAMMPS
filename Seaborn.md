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
sns.barplot(x= " " ,y=" ",data=      ,hue=" ",
