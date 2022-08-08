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

# Day 2

Open the file README.md located in openlane configuration
![](Imagenes/Img-2022-08-07-22-01-03.png)
![](Imagenes/Img-2022-08-07-22-02-58.png)

run_floorplan
![](Imagenes/Img-2022-08-08-00-32-32.png)

![](Imagenes/Img-2022-08-08-00-38-02.png)

![](Imagenes/Img-2022-08-08-01-54-57.png)

![](Imagenes/Img-2022-08-08-02-03-07.png)

![](Imagenes/Img-2022-08-08-02-05-10.png)

run_placement
![](Imagenes/Img-2022-08-08-02-24-04.png)

`magic -T /home/carlos.boada/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130A.tech lef read ../../tmp/merged.lef def read picorv32a.placement.def &`


![](Imagenes/Img-2022-08-08-02-34-36.png)

![](Imagenes/Img-2022-08-08-02-38-55.png)
# Day 3

The file is cloned in the openlane folder 
`git clone https://github.com/nickson-jose/vsdstdcelldesign.git`

![](Imagenes/Img-2022-08-07-23-41-12.png)

then copy the file sky130A.tech in the current folder and proceed to launch

`magic -T sky130A.tech sky130_inv.mag &`
![](Imagenes/Img-2022-08-07-23-58-37.png)




