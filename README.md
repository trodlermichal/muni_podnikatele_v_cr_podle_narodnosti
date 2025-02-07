# MUNI kurz Data Kolem nás  
## Podnikatelé v ČR podle národností  
  
Stažení, čištění, shromáždění a analýza proměny počtu podnikatelů v ČR podle národností. Data jsou stažena z [Ministerstva Obchodu a Průmyslu](https://mpo.gov.cz/cz/podnikani/zivnostenske-podnikani/statisticke-udaje-o-podnikatelich/pocty-podnikatelu-dle-obcanstvi-podnikajicich-v-ceske-republice--151024/). 100% Python, Jupyter notebook.  
  
###[Scraper.ipynb](scraper.ipynb)  
- [x] Inicializace git repozitáře a Jupyter notebooku  
- [x] Stažení dat pomocí scraperu (Playwright async) - 34 záznamů  
- [x] Převod .xlsx souborů se zamčenými listy do csv  

### Preprocessing.ipynb
- [x] Manuální upravení názvů "Text" na "YYYY QQ"  
- [x] Preprocessing vzniklých CSV
    - Přejmenování sloupců, odstranění zbytečných sloupců a řádků, nastavení indexu
- [x] Vytvoření listů all_sums a all_dataframes  
- [x] Merge (left outter join) do jednoho  

### Visualisation.ipynb
- [x] Vizualizace pomocí matplotlib
    - Stacked Area Chart
    - Line Chart
    - 100% Stacked Area Chart
- [x] Interaktivní vizualizace na Datawrapper.de

<iframe title="Změna počtu podnikatelů v ČR" aria-label="Interactive line chart" id="datawrapper-chart-9vA7d" src="https://datawrapper.dwcdn.net/9vA7d/1/" scrolling="no" frameborder="0" style="width: 0; min-width: 100% !important; border: none;" height="591" data-external="1"></iframe><script type="text/javascript">!function(){"use strict";window.addEventListener("message",(function(a){if(void 0!==a.data["datawrapper-height"]){var e=document.querySelectorAll("iframe");for(var t in a.data["datawrapper-height"])for(var r=0;r<e.length;r++)if(e[r].contentWindow===a.source){var i=a.data["datawrapper-height"][t]+"px";e[r].style.height=i}}}))}();
</script>
