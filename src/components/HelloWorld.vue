<template>
  <div>
    <div class="entry-header">
      <span class="post-category"
        ><a title="Tendencias">Spotify: tendencias musicales</a></span
      >
      <h3 class="entry-title">
        <a title="Lenguaje universal">¿LENGUAJE UNIVERSAL?</a>
      </h3>
    </div>
    <div class="document">
      <!--Paragraph 1: Presenting both sides of general phenomena-->
      <p style="text-align: justify">
        Cuenta una famosa leyenda bíblica que ninguna empresa sería imposible a
        los hombres si éstos hablaban una misma lengua: el pueblo del mundo,
        cuando era uno solo y decía con las mismas palabras, decidió construir
        una torre tan alta que llegara al cielo. Dicha soberbia despertó la ira
        de Dios, y éste, sabiendo donde estaba la fuerza de los hombres, hizo
        que comenzaran a hablar diferentes lenguas para que dejaran de
        entenderse y se disgregaran por el mundo. La Torre de Babel cayó, y para
        siempre el mundo se convirtió en una canción arrítmica, hecha a hermosos
        retazos anacrónicos.
      </p>
      <p style="text-align: justify">
        Como una constumbre milenaria, el hombre parece seguir desafiando los
        designios del Todopoderoso y, aún hoy, sigue intentando levantar su
        Torre de Babel. Al nuevo modo de hablar con las mismas palabras le
        llamamos hoy
        <b>globalización</b>.
      </p>
      <p style="text-align: justify">
        En la actualidad la <b>globalización</b> es uno de los temas más
        controversiales para las ciencias sociales y humanísticas. Un primer
        enfoque sugiere al fenómeno como responsable de una reducción del
        potencial creativo del mundo, mientras que algunos estudiosos afirman
        que la circulación de prácticas culturales promoverá la
        <b>diversidad</b> y el pluralismo.
      </p>

      <!--Paragraph 2: Particular impact of general phenomena in main topic-->
      <p style="text-align: justify">
        Ninguna manifestación humana parece englobar esta dicotomía de una
        manera tan simbólica y singular como la <b>música</b>. Casi cualquier
        ritmo que conocemos hoy es el resultado de un proceso de
        <b>transculturación</b> derivado del impacto del flujo migratorio y el
        desarrollo de las <b>comunicaciones</b>: imaginen por un momento la
        sorpresa de Bethoveen al escuchar como su 5ta sinfonía desemboca en el
        inconfundible alarido de Dámaso Pérez Prado, escuchen al pueblo moro en
        el lamento de un tablao flamenco, sientan la explosión de libertad
        contenida en los tambores de nuestra música negra.
      </p>

      <!--Paragraph 3: Choosing sides-->
      <p style="text-align: justify">
        La globalización musical ha tratado, fundamentalmente, del crecimiento
        del
        <b>intercambio y la conexión</b>. La posibilidad que nos brinda la
        <b>tecnología</b> de llevar nuestra música a todas partes ha sido una
        vía de escape del <b>imperialismo cultural</b> y las autoridades de
        control del mercado musical. La migración, como motor impulsor de las
        primeras manifestaciones de transculturación, ha llevado de un lugar a
        otro las nostalgias musicales de cada país. La
        <b>apertura de espacios</b> comunes ha ampliado el espectro de ritmos y
        ha promovido la <b>aceptación</b> en el mercado de formas novedosas de
        hacer música. Somos todos diferentes, pero hemos encontrado la manera de
        abrir un túnel invisible para decirnos cuán diferentes somos. Ahí radica
        la fuerza necesaria para poner el último ladrillo en nuestra Torre de
        Babel.
      </p>

      <!--Paragraph 4: Presenting spotify as source-->
      <p style="text-align: justify">
        Para ponernos a tono con el tema que tratamos, no podemos obviar a las
        nuevas tecnologías de la información y la comunicación como arítifices
        fundamentales de la construcción de ese túnel, y si se habla de
        plataformas de <i>streaming</i> de música es obligatorio mencionar a
        <b>Spotify</b>. Con una base de suscriptores que <b>asciende</b> de 207
        millones de usuarios mensuales en 2018 a <b>217 millones</b> en 2019
        (con un crecimiento a usuarios de pago de 31%); <b>Spotify</b> sugiere
        una <b>confiable</b> fuente de información acerca de
        <b>tendencias</b> musicales globales y demuestra que cada día estamos
        más conectados para compartir nuestro contexto musical.
      </p>

      <!--Paragraph 5: Presenting data supporting previous statement. General analysis of data through interactive map-->
      <p style="text-align: justify">
        La globalización no se trata de un mero acercamiento al balance, sino que muestra 
        a la cultura anglosajona como pauta de la industria musical. Si bien el Reino Unido 
        comenzó el trabajo dejándonos el legado de quienes 
        se llamaron más famosos que Dios, o de quienes hallaron simpatía por el Diablo; 
        ha sido América del Norte quien se ha consolidado como la vanguardia de lo más escuchado en los últimos tiempos. 
        La mundialización e internacionalización constituyen procesos direccionales: es mucho más fuerte el flujo de 
        influencia cultural desde quienes tienen las herramientas adecuadas hacia quienes esperan con los brazos abiertos
        cualquier soplo de primermundismo.  
      </p>
      <p style="text-align: justify">
        Por otro lado, la riqueza y diversidad de los ritmos latinoamericanos ha mostrado cierta resistencia a 
        ser absorbida por los tentáculos del mercado mundial: la penetración es innegable, pero no absoluta.
      </p>
      
      <div class="entry-cover"  style="margin-top:8px">
        <div class="post-meta">
          <select v-model="selectedDateGlobal">
            <option disabled value="">Seleccione una fecha</option>
            <option v-for="d in getDates" :key="d">{{ d }}</option>
          </select>
          <div class="hello" ref="chartdivGlobal"></div>
        </div>
      </div>
      <p style="text-align: justify">
        Pero... </br>
          ¿en qué punto del fenómeno nos encontramos? 
        </br>
        Hasta ahora hemos 
        demostrado que el mundo se agrupa en comunidades culturales, 
        pero un resultado aún más interesante nos conduce a pensar que la fusión de la 
        tendencia musical se desarrolla por niveles. Estamos en un momento donde 
        se han formado las principales congregaciones a través de la mezcla de elementos con puntos comunes:
        dígase historias enlazadas, lenguas similares o geografías hermanas.</br>
        ¿Cuál será el <b>siguiente nivel</b>?
      </p>
      
      <p style="text-align: justify">        
        Si observamos el crecimiento de la similitud entre los grupos representativos con el centro global, éste nos sugiere 
        que el próximo paso será la <b>fusión</b> del cada una de los conjuntos, para vislumbrar el punto final de
        la globalización: la formación de una única comunidad universal. El proceso parece desarrollarse
        de forma similar en cada uno de los niveles: las uniones se realizan a partir de los mismos criterios.
      </p>
      <div class="entry-cover" style="margin-top:8px">
        <div class="post-meta">
          <select v-model="selectedDate">
            <option disabled value="">Seleccione una fecha</option>
            <option v-for="d in getDates" :key="d">{{ d }}</option>
          </select>
          <div class="hello" ref="chartdiv"></div>
        </div>
      </div>

      <p style="text-align: justify">
        La <b>cercanía geográfica y cultural</b> es un factor influyente en la
        similitud de tendencias musicales. Países de histórico
        <b>intercambio</b> cultural y migratorio como EEUU, Canadá, Reino Unido
        y Australia poseen los <b>más altos</b> índices de similitud mutua y se
        agrupan junto a Sudáfrica, un
        país africano que se acerca mucho al estándar anglosajón. También,
        probablemente como resultado de la colonización y de la lengua común, España se encuentra
        junto a América Central y América del Sur en otro de los
        grupos. En la muestra europea seleccionada, se observan
        similares distribuciones de índices: países que
        <b>comparten fronteras</b> como Alemania, Austria y Suiza o
        <b>raíces lingüísticas comunes</b> Argentina, Italia, Chile y España;
        forman las componentes más homogéneas. Otro clúster está compuesto por
        Indonesia, Taiwan, Vietnam, Tailandia, Filipinas y Malasia; apoyando la
        hipótesis de que países cercanos geográfica y culturalmente tendrán
        gustos musicales similares.
      </p>

      <p style="text-align: justify">
        El país <b>más singular</b> es Brasil, con un discreto promedio de
        similaridad; consistente con su condición de
        <b>potencia cultural</b> con una fuerte industria musical nacional.
      </p>

      <p style="text-align: justify">
        La <b>occidentalización</b> de Japón, con una distribución general de
        similitud que no se presenta diferente a la de cualquier otra potencia,
        demuestra nuevamente a Occidente como núcleo de la tendencia musical.
      </p>
      
      <p style="text-align: justify">
        Si hacemos un análisis que va de lo general a lo particular, nos queda 
        definir si en los grupos se mantienen las diferencias, o se lleva a cabo 
        un proceso de micro-fusión. 
      </p>
      <radarchart />
      <p style="text-align: justify">
        Si comparamos los niveles de similitud interna a lo largo del tiempo, 
        podemos constatar que evidentemente se produce una homogeneización de los grupos, 
        especialmente de los representativos de ciertas pautas culturales universales. 
        Podemos extraer también que existen naciones más resistentes a la penetración, 
        y que se agrupan como las ovejas negras del rebaño para mantener un discreto crecimiento 
        de las similitudes internas.  
      </p>
      <p style="text-align: justify">
      En conclusión, podemos decir que la música en tendencia queda categorizada dentro de una 
      etiqueta acuñada como <i>world music</i>, que engloba simbólicamente nuestro capricho 
      por hablar la misma lengua. 
      Los ritmos originales se deforman y se fusionan para crear un cuerpo musical que se aleja
      de su génesis multicolor para perderse eternamente en la universalidad. 
      La cultura, en su papel estructurador de la sociedad, es consistente con las estructuras de poder 
      convencionales. 
      La eficiencia del mercado musical necesita del concurso de la globalización para cumplir sus objetivos:
      las fronteras dejarán de ser un límite para la hegemonía cultural. 
      </p>
    </div>
  </div>
</template>

<script>
import * as am4core from "@amcharts/amcharts4/core";
import * as am4maps from "@amcharts/amcharts4/maps";
import am4geodata_worldLow from "@amcharts/amcharts4-geodata/worldLow";
import clustering from "../assets/clustering.json";
import globalSimilarity from "../assets/global_similarity.json";
import RadarChart from "./RadarChart.vue";

export default {
  name: "HelloWorld",
  components: {
    radarchart: RadarChart,
  },
  data() {
    return {
      selectedDate: "",
      selectedDateGlobal: "",
      colors: ["#2c28a1", "#28a15a", "#a14c28", "#95a128"],
      gradientColors: [
        "#167DAB",
        "#2D7798",
        "#447185",
        "#5B6B72",
        "#72655F",
        "#895E4C",
        "#A05839",
        "#B75226",
        "#CE4C13",
        "#E54600",
      ],
      chart: null,
      polygonSeries: null,
      // Radar chart
      series: [
        {
          name: "Series 1",
          data: [80, 50, 30, 40, 100, 20],
        },
      ],
      chartOptions: {
        chart: {
          height: 350,
          type: "radar",
        },
        title: {
          text: "Basic Radar Chart",
        },
        xaxis: {
          categories: ["January", "February", "March", "April", "May", "June"],
        },
      },
    };
  },
  mounted() {
    this.chart = am4core.create(this.$refs.chartdiv, am4maps.MapChart);
    this.chart.geodata = am4geodata_worldLow;
    this.chart.projection = new am4maps.projections.Miller();
    this.polygonSeries = this.chart.series.push(new am4maps.MapPolygonSeries());
    this.polygonSeries.useGeodata = true;
    this.polygonSeries.mapPolygons.template.events.on("hit", function (ev) {
      this.chart.zoomToMapObject(ev.target);
    });
    this.polygonSeries.exclude = ["AQ"];
    var polygonTemplate = this.polygonSeries.mapPolygons.template;
    polygonTemplate.tooltipText = "{name}";
    polygonTemplate.fill = am4core.color("#bac6cc");
    polygonTemplate.tooltipText = "{name}: {value}";
    this.polygonSeries.data = this.serieClustering;
    polygonTemplate.propertyFields.fill = "fill";

    this.chart2 = am4core.create(this.$refs.chartdivGlobal, am4maps.MapChart);
    this.chart2.geodata = am4geodata_worldLow;
    this.chart2.projection = new am4maps.projections.Miller();
    this.polygonSeries2 = this.chart2.series.push(
      new am4maps.MapPolygonSeries()
    );
    this.polygonSeries2.useGeodata = true;
    this.polygonSeries2.mapPolygons.template.events.on("hit", function (ev) {
      this.chart2.zoomToMapObject(ev.target);
    });
    this.polygonSeries2.exclude = ["AQ"];
    var polygonTemplate2 = this.polygonSeries2.mapPolygons.template;
    polygonTemplate2.tooltipText = "{name}";
    polygonTemplate2.fill = am4core.color("#bac6cc");
    polygonTemplate2.tooltipText = "{name}: {value}";
    this.polygonSeries2.data = this.serieHeatMap;
    polygonTemplate2.propertyFields.fill = "fill";
  },
  watch: {
    serieClustering: function (val) {
      this.polygonSeries = this.chart.series.push(
        new am4maps.MapPolygonSeries()
      );
      this.polygonSeries.useGeodata = true;
      this.polygonSeries.mapPolygons.template.events.on("hit", function (ev) {
        this.chart.zoomToMapObject(ev.target);
      });
      this.polygonSeries.exclude = ["AQ"];
      var polygonTemplate = this.polygonSeries.mapPolygons.template;
      polygonTemplate.tooltipText = "{name}";
      polygonTemplate.fill = am4core.color("#bac6cc");
      polygonTemplate.tooltipText = "{name}: {value}";
      this.polygonSeries.data = val;
      polygonTemplate.propertyFields.fill = "fill";
    },
    serieHeatMap: function (val) {
      this.polygonSeries2 = this.chart2.series.push(
        new am4maps.MapPolygonSeries()
      );
      this.polygonSeries2.useGeodata = true;
      this.polygonSeries2.mapPolygons.template.events.on("hit", function (ev) {
        this.chart2.zoomToMapObject(ev.target);
      });
      this.polygonSeries2.exclude = ["AQ"];
      var polygonTemplate2 = this.polygonSeries2.mapPolygons.template;
      polygonTemplate2.tooltipText = "{name}";
      polygonTemplate2.fill = am4core.color("#bac6cc");
      polygonTemplate2.tooltipText = "{name}: {value}";
      this.polygonSeries2.data = val;
      polygonTemplate2.propertyFields.fill = "fill";
    },
  },
  computed: {
    getDates() {
      var dates = [];
      clustering.forEach((c) => {
        dates.push(c.date);
      });
      return dates;
    },
    serieClustering() {
      var serie = [];
      clustering.forEach((c) => {
        if (c.date == this.selectedDate) {
          for (let i = 0; i < c.clus.length; i++) {
            const cl = c.clus[i];
            cl.forEach((e) => {
              serie.push({
                id: e,
                value: i + 1,
                fill: this.colors[i],
              });
            });
          }
        }
      });
      return serie;
    },
    serieHeatMap() {
      var serie = [];
      var regions = globalSimilarity[this.selectedDateGlobal];
      if (regions != null) {
        Object.keys(regions).forEach((r) => {
          var v = regions[r];
          serie.push({
            id: r,
            value: v,
            fill: this.gradientColors[v],
          });
        });
      }
      console.log(serie);
      return serie;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  width: 100%;
  height: 500px;
}

.document {
  margin-left: 150pt;
  margin-right: 150pt;
  margin-bottom: 50pt;
}
</style>