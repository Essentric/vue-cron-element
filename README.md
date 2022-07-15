# 示例:
````html
  <el-dialog title="Cron表达式生成器" :visible.sync="openCron" append-to-body destroy-on-close class="scrollbar">
    <crontab :expression="expression" @hide="openCron=false" @fill="crontabFill" />
  </el-dialog>
`````