<template>
  <div class="container">
    <nav-bar />
    <banner
      title="Fun Facts"
      subtitle="Baby Name @UK"
    />
    <section class="section">
      <div class="columns">
        <div class="column is-8 is-offset-2" style="text-align: left;">
          <router-link :to="'/articles'" class="">Back to Article List</router-link>
          <div class="card">
            <header class="card-header">
              <p class="card-header-title" style="justify-content: center;">
                Do you know...
              </p>
            </header>
            <div class="card-content" style="text-align: justify;">
              <ol>
                <li v-for="item in facts" v-html="item">
                </li>
              </ol>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import NavBar from '../components/NavBar'
import Banner from '../components/Banner'
export default {
  name: 'fun-facts-page',
  components: {
    NavBar, Banner
  },
  data () {
    return {
      facts: ['Parents in UK tend to prefer to choose <span class="emph">more unpopular</span> names for their children.', 'The percentage of top 100 names in England and Wales has dropped from <span class="emph">51%</span> in 2010 to reach rock bottom in 2015 by <span class="emph">47%</span>.', 'The percentage of top 100 names in Scotland has dropped from <span class="emph">59%</span> in 2010 to reach rock bottom in 2015 by <span class="emph">55%</span>.', 'The percentage of top 100 names in Northern Ireland has dropped from <span class="emph">64%</span> in 2010 to reach rock bottom in 2015 by <span class="emph">59%</span>.', 'In 2010, <span class="emph">51%</span> of babies in England and Wales have names from the top 100 popular names.', 'In 2015, <span class="emph">47%</span> of babies in England and Wales have names from the top 100 popular names.', 'From 2010 to 2015, The average percentage of babies who were named by one of the top 100 names in England and Wales is <span class="emph">49%</span>.', 'In 2010, the percentage of baby boys in England and Wales is <span class="emph">55.8%</span> while this percentage has increased to stand at <span class="emph">56.3%</span> in 2015.', 'In 2010, the percentage of baby girls in England and Wales is <span class="emph">44.2%</span> while this percentage has decreased to stand at <span class="emph">43.7%</span> in 2015.', 'In Scotland, the average number of baby boys who were named from top 100 popular names is <span class="emph">60%</span>.', 'In Scotland, the average number of baby girls who were named from top 100 popular names is <span class="emph">53%</span>.', 'In Scotland, the average number of babies who were named from top 100 popular names is <span class="emph">57%</span>.', 'The highest number of births for baby boys in Scotland was in 2011 by <span class="emph">30,111</span> babies.', 'The lowest number of births for baby girls in Scotland was in 2015 by <span class="emph">26,746 babies.</span>', 'The number of births has declined in Scotland from <span class="emph">58,781</span> babies in 2010 to <span class="emph">55100</span> babies in 2015.', 'In 2010, the percentage of baby boys in Scotland was <span class="emph">50.8%</span> while the percentage of baby girls is <span class="emph">49.2%</span>.', 'In 2015, the percentage of baby boys in Scotland was <span class="emph">51.5%</span> while the percentage of baby girls is <span class="emph">48.5%</span>.', 'In Northern Ireland, the average percentage of baby boys is <span class="emph">53.7%</span> while the average percentage of baby girls is <span class="emph">46.3%</span>.', 'From 2010 to 2015, The average percentage of babies who were named by one of the top 100 names in Northern Ireland is <span class="emph">61.6%</span>.', 'The highest number of births in Northern Ireland was in 2011 by <span class="emph">25,315</span> babies.', 'In Northern Ireland, <span class="emph">25,273</span> babies were born in 2011 while <span class="emph">25,269</span> babies were born in 2012.']
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style: none;
}

a {
  color: #42b983;
}

a:hover {
  text-decoration: underline;
}
li {
  margin: 7px 10px;
}
</style>
