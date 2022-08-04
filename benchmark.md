## Minecraft load time benchmark


---

<p align="center" style="font-size:160%;">
MC total load time:<br>
712.45 sec
<br>
<sup><sub>(
11:52 min
)</sub></sup>
</p>

<br>


<p align="center">
<img src="https://quickchart.io/chart?w=400&h=30&c={%20type:%20'horizontalBar',%20data:%20{%20datasets:%20[%20{label:%20'MODS:',%20data:%20[404.36]},%20{label:%20'FML%20stuff:',%20data:%20[308.09]}%20]%20},%20options:%20{%20scales:%20{%20xAxes:%20[{display:%20false,stacked:%20true}],%20yAxes:%20[{display:%20false,stacked:%20true}],%20},%20elements:%20{rectangle:%20{borderWidth:%202}},%20legend:%20{display:%20false,},%20plugins:%20{datalabels:%20{color:%20'white',formatter:%20(value,%20context)%20=>%20[context.dataset.label,%20value].join('%20')%20}}%20}%20}"/>
</p>

<br>

# Mods Loading Time
<p align="center">
<img src="https://quickchart.io/chart?w=400&h=300&c={%20type:%20'outlabeledPie',%20options:%20{%20cutoutPercentage:%2025,%20plugins:%20{%20legend:%20!1,%20outlabels:%20{%20stretch:%205,%20padding:%201,%20text:%20(v,i)=>[%20v.labels[v.dataIndex],'%20',%20(v.percent*1000|0)/10,%20String.fromCharCode(37)].join('')%20}%20}%20},%20data:%20{...%20`%20436e17%2074.96s%20Had%20Enough%20Items;%20214d9e%2032.39s%20Minecraft%20Forge;%20516fa8%2013.97s%20Ender%20IO;%208c2ccd%2011.31s%20Immersive%20Engineering;%20a651a8%209.59s%20IndustrialCraft%202;%208f3087%209.10s%20Forge%20Mod%20Loader;%20cd2c9f%208.08s%20Ancient%20Warfare%20Structures;%208f3041%208.07s%20Tech%20Reborn;%2099ba3e%207.90s%20Ancient%20Warfare%20NPCs;%20219e2a%207.65s%20BuildCraft%20Lib;%209d2ccd%207.36s%20Immersive%20Intelligence;%20538f30%207.26s%20Animania;%208f304e%206.09s%20Astral%20Sorcery;%206e175e%205.62s%20Recurrent%20Complex;%20216364%205.24s%20Thermal%20Expansion;%208f6c30%205.05s%20Dynamic%20Surroundings;%202c6ccd%205.04s%20AgriCraft;%205fba3e%204.21s%20Modular%20Machinery;%206e176a%204.20s%20Unlimited%20Chisel%20Works;%2051a8a8%203.89s%20Ore%20Stone%20Variants;%20444444%2074.14s%2045%20Other%20mods;%20333333%2082.46s%20243%20'Fast'%20mods%20(load%201.0s%20-%200.1s);%20222222%2010.79s%20335%20'Instant'%20mods%20(load%20%3C%200.1s)%20`%20.split(';').reduce((a,%20l)%20=>%20{%20l.match(/(\w{6})%20*(\d*\.\d*)s%20(.*)/)%20.slice(1).map((a,%20i)%20=>%20[[String.fromCharCode(35),a].join(''),%20parseFloat(a),%20a][i])%20.forEach((s,%20i)%20=>%20[a.datasets[0].backgroundColor,%20a.datasets[0].data,%20a.labels][i].push(s)%20);%20return%20a%20},%20{%20labels:%20[],%20datasets:%20[{%20backgroundColor:%20[],%20data:%20[],%20borderColor:%20'rgba(22,22,22,0.3)',%20borderWidth:%201%20}]%20})%20}%20}"/>
</p>

<br>

# Top Mods Details (except JEI, FML and Forge)
<p align="center">
<img src="https://quickchart.io/chart?w=400&h=450&c={%20options:%20{%20scales:%20{%20xAxes:%20[{stacked:%20true}],%20yAxes:%20[{stacked:%20true}],%20},%20plugins:%20{%20datalabels:%20{%20anchor:%20'end',%20align:%20'top',%20color:%20'white',%20backgroundColor:%20'rgba(46,%20140,%20171,%200.6)',%20borderColor:%20'rgba(41,%20168,%20194,%201.0)',%20borderWidth:%200.5,%20borderRadius:%203,%20padding:%200,%20font:%20{size:10},%20formatter:%20(v,ctx)%20=>%20ctx.datasetIndex!=ctx.chart.data.datasets.length-1%20?%20null%20:%20[((ctx.chart.data.datasets.reduce((a,b)=>a-%20-b.data[ctx.dataIndex],0)*10)|0)/10,'s'].join('')%20},%20colorschemes:%20{%20scheme:%20'office.Damask6'%20}%20}%20},%20type:%20'bar',%20data:%20{...(()%20=>%20{%20let%20a%20=%20{%20labels:%20[],%20datasets:%20[]%20};%20`%201:%20Construction;%202:%20Loading%20Resources;%203:%20PreInitialization;%204:%20Initialization;%205:%20InterModComms$IMC;%206:%20PostInitialization;%207:%20LoadComplete;%208:%20ModIdMapping%20`%20.split(';')%20.map(l%20=>%20l.match(/\d:%20(.*)/).slice(1))%20.forEach(([name])%20=>%20a.datasets.push({%20label:%20name,%20data:%20[]%20}));%20`%201%202%203%204%205%206%207%208%20;%20Had%20Enough%20Items%20|%200.04|%200.00|%201.78|%200.03|%200.00|%200.00|%2073.10|%200.00;%20Ender%20IO%20|%201.08|%200.01|%202.01|%200.30|%206.10|%200.13|%200.00|%204.34;%20Immersive%20Engineering%20|%200.56|%200.01|%200.74|%200.32|%200.00|%209.68|%200.00|%200.00;%20IndustrialCraft%202%20|%200.44|%200.02|%207.03|%200.68|%200.00|%201.43|%200.00|%200.00;%20Ancient%20Warfare%20Structures%20|%200.05|%200.03|%200.16|%200.04|%200.00|%207.81|%200.00|%200.00;%20Tech%20Reborn%20|%200.04|%200.01|%203.61|%201.77|%200.00|%202.64|%200.00|%200.00;%20Ancient%20Warfare%20NPCs%20|%200.07|%200.04|%200.19|%200.00|%200.00|%207.61|%200.00|%200.00;%20BuildCraft%20Lib%20|%200.03|%200.01|%200.54|%200.07|%200.00|%207.00|%200.00|%200.00;%20Immersive%20Intelligence%20|%201.03|%200.01|%202.25|%200.53|%200.00|%203.54|%200.00|%200.00;%20Animania%20|%200.17|%200.00|%202.50|%200.07|%200.00|%204.52|%200.00|%200.00;%20Astral%20Sorcery%20|%200.13|%200.01|%204.53|%200.73|%200.00|%200.70|%200.00|%200.00;%20Recurrent%20Complex%20|%200.14|%200.01|%200.41|%200.57|%200.00|%204.50|%200.00|%200.00%20`%20.split(';').slice(1)%20.map(l%20=>%20l.split('|').map(s%20=>%20s.trim()))%20.forEach(([name,%20...arr],%20i)%20=>%20{%20a.labels.push(name);%20arr.forEach((v,%20j)%20=>%20a.datasets[j].data[i]%20=%20v)%20});%20return%20a%20})()}%20}"/>
</p>

<br>

# TOP JEI Registered Plugis
<p align="center">
<img src="https://quickchart.io/chart?w=700&c={%20options:%20{%20elements:%20{%20rectangle:%20{%20borderWidth:%201%20}%20},%20legend:%20false%20},%20type:%20'horizontalBar',%20data:%20{...(()%20=>%20{%20let%20a%20=%20{%20labels:%20[],%20datasets:%20[{%20backgroundColor:%20'rgba(0,%2099,%20132,%200.5)',%20borderColor:%20'rgb(0,%2099,%20132)',%20data:%20[]%20}]%20};%20`%200.00:%20Other%20-15%20Plugins%20`%20.split(';')%20.map(l%20=>%20l.split(':'))%20.forEach(([time,%20name])%20=>%20{%20a.labels.push(name);%20a.datasets[0].data.push(time)%20})%20;%20return%20a%20})()%20}%20}"/>
</p>

<br>

# FML Stuff
<p align="center">
<img src="https://quickchart.io/chart?w=500&h=400&c={%20options:%20{%20rotation:%20Math.PI,%20cutoutPercentage:%2055,%20plugins:%20{%20legend:%20!1,%20outlabels:%20{%20stretch:%205,%20padding:%201,%20text:%20(v)=>v.labels%20},%20doughnutlabel:%20{%20labels:%20[%20{%20text:%20'FML%20stuff:',%20color:%20'rgba(128,%20128,%20128,%200.5)',%20font:%20{size:%2018}%20},%20{%20text:%20[308.09,'s'].join(''),%20color:%20'rgba(128,%20128,%20128,%201)',%20font:%20{size:%2022}%20}%20]%20},%20}%20},%20type:%20'outlabeledPie',%20data:%20{...(()%20=>%20{%20let%20a%20=%20{%20labels:%20[],%20datasets:%20[{%20backgroundColor:%20[],%20data:%20[],%20borderColor:%20'rgba(22,22,22,0.3)',%20borderWidth:%202%20}]%20};%20`%20993A00%203.88s%20Loading%20sounds;%20994400%203.95s%20Loading%20Resource%20-%20SoundHandler;%20994F00%2043.37s%20ModelLoader:%20blocks;%20995900%2016.41s%20ModelLoader:%20items;%20996300%2030.99s%20ModelLoader:%20baking;%20996D00%200.72s%20Applying%20remove%20recipe%20actions;%20997700%200.00s%20Applying%20remove%20furnace%20recipe%20actions;%20998200%204.04s%20Indexing%20ingredients;%20444444%20204.73s%20Other%20`%20.split(';')%20.map(l%20=>%20l.match(/(\w{6})%20*(\d*\.\d*)s%20(.*)/))%20.forEach(([,%20col,%20time,%20name])%20=>%20{%20a.labels.push([name,%20'%20',%20time,%20's'].join(''));%20a.datasets[0].data.push(parseFloat(time));%20a.datasets[0].backgroundColor.push([String.fromCharCode(35),%20col].join(''))%20})%20;%20return%20a%20})()}%20}"/>
</p>

<br>
