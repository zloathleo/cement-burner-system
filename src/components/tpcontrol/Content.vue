<template>

  <div class="columns">

    <div class="column is-6">

      <div class="card card-bg-transparent" style="box-shadow: none;padding-bottom: 2rem;">
        <div class="card-header color-primary-4">
          探头状态显示
        </div>
        <div class="card-content-table">
          <table class="table is-bordered  is-fullwidth card-bg-transparent">
            <tbody>
              <tr>
                <td class="table-td">电源启动</td>
                <td class="table-td">就地</td>
                <td class="table-td"></td>
                <td class="table-td"></td>
              </tr>
              <tr>
                <td class="table-td">吹扫风低压报警</td>
                <td class="table-td">冷却风低压报警</td>
                <td class="table-td">冷却风高压报警</td>
                <td class="table-td">温度场探头温度高报警</td>
              </tr>
              <tr>
                <td class="table-td">温度场探头A进</td>
                <td class="table-td">温度场探头A退</td>
                <td class="table-td">温度场探头B进</td>
                <td class="table-td">温度场探头B退</td>
              </tr>
              <tr>
                <td class="table-td">温度场探头A正常</td>
                <td class="table-td"> </td>
                <td class="table-td">温度场探头B正常</td>
                <td class="table-td"> </td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>

      <div class="card card-bg-transparent" style="box-shadow: none;padding-bottom: 2rem;">
        <div class="card-header color-primary-4">
          探头控制操作
        </div>
        <div class="card-content-table">
          <table class="table is-bordered  is-fullwidth card-bg-transparent">
            <tbody>
              <tr>
                <td class="table-td">探头A允许进</td>
                <td class="table-td">不允许原因</td>
                <td class="table-td">进</td>
                <td class="table-td">退</td>
              </tr>
              <tr>
                <td class="table-td">探头B允许进</td>
                <td class="table-td">不允许原因</td>
                <td class="table-td">进</td>
                <td class="table-td">退</td>
              </tr>
              <tr>
                <td class="table-td">探头允许上电</td>
                <td class="table-td">不允许原因</td>
                <td class="table-td">上电</td>
                <td class="table-td">断电</td>
              </tr>
              <tr>
                <td class="table-td">风机允许开</td>
                <td class="table-td">不允许原因</td>
                <td class="table-td">开</td>
                <td class="table-td">关</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>

    </div>

    <div class="column is-6">
      <div class="card card-bg-transparent" style="box-shadow: none;padding-bottom: 2rem;">
        <div class="card-header color-primary-4">
          Temperature pattern
        </div>
        <div class="card-content-table">
          <table class="table is-bordered  is-fullwidth card-bg-transparent">
            <tbody>
              <tr>
                <td class="table-td-left">Three</td>
                <td class="table-td">Four</td>
              </tr>
              <tr>
                <td class="table-td-left">Five</td>
                <td class="table-td">Six</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>

  </div>

</template>

<style scoped lang="less">
</style>

<script> 
export default {
  components: {
  },
  data() {
    return {
      commondata: {
        d1: "-",
        d2: "-",
        d3: "-",
        d4: "-",
      },
      data: {},
    }
  },
  mounted() {
    let _this = this;


  },
  methods: {

  }
}
</script>
