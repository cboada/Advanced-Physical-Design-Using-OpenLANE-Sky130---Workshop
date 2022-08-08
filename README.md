# Advanced-Physical-Design-Using-OpenLANE-Sky130-Workshop
Repository corresponding to the work carried out in the VSD-IAT SKY130/Physical Design Workshop during 5 days of the month of August 2022

# Day 1

`Desktop/work/tools/openlane_working_dir/openlane$ ls -ltr`

![](Imagenes/Img-2022-08-07-19-15-34.png)


`&docker`

`bash-4.2$./flow.tcl -interactive` 
![](Imagenes/Img-2022-08-07-19-29-15.png)

`%package require openlane 0.9`

`%prep -design picorv32a`
![](Imagenes/Img-2022-08-07-19-51-42.png)

`run_synthesis`

![](Imagenes/Img-2022-08-07-20-37-59.png)
--
![](Imagenes/Img-2022-08-07-20-39-11.png)

$$\textit{Number of cells}=14876$$ 

$$\textit{Total number of flops}=1613$$

$$\textit{Flop ration}:(\textit{Total number of flops}/\textit{Number of cells})*100=10.84$$

$$buf_1=1656$$

$$buf_2=8$$

$$ \textit{Buffer ratio}: \frac{(buf_1+buf_2)}{\textit{Number of cells}}=11.18$$ 