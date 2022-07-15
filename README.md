# 示例:
````JavaScript
  import CronTab from './index.vue'

  components: { CronTab },
  data() {
    return {
      expression: '',
      openCron: false
    }
  },
  methods: {
    crontabFill(value) {
      this.expression = value
    }
  }
````
````html
  <el-dialog title="Cron表达式生成器" :visible.sync="openCron" append-to-body destroy-on-close class="scrollbar">
    <crontab :expression="expression" @hide="openCron=false" @fill="crontabFill" />
  </el-dialog>
`````
