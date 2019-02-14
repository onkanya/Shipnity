<template>
  <div id="app">
    <el-container>
        <el-header class="m-navbar">
            <h1>Shipnity</h1>
        </el-header>
        <el-main class="m-content">
            <el-row>
                ราคาแพ็คเก็จ  (เลือกให้ดีที่สุดฉบับธุรกิจคุณ)
            </el-row>
            <el-row>
                * ตัวแทนจำหน่ายของร้าน สามารถมี user ของตัวเองเพื่อเข้ามาสร้างออร์เดอร์, เช็คสต็อก, ดูประวัติ, ยอดขายของตัวเองได้
            </el-row>
            <el-row>
                <el-col class="m-subcontent">
                    <el-row :gutter="20" justify="space-between" align="middle">
                        <!-- Image -->
                        <el-col :xs="24" :sm="12" :md="12" :lg="12">
                            <div class="image">
                                Image
                            </div>
                        </el-col>
                        <!-- Text -->
                        <el-col :xs="24" :sm="6" :md="6" :lg="6" class="m-side-detail">
                            <el-row>
                                <el-col :span="24">
                                    สมัครวันนี้ ฟรีทันที 50 ออร์เดอร์
                                </el-col>
                            </el-row>                            
                            <el-row>
                                <el-col :span="24">
                                    - ใช้งานฟรีตลอดไป
                                </el-col>
                            </el-row>                            
                            <el-row>
                                <el-col :span="24">
                                    - ไม่จำกัดฟีเจอร์
                                </el-col>
                            </el-row>                            
                            <el-row>
                                <el-col :span="24">
                                    ขายของครบเครื่องทุกฟังก์ชัน
                                </el-col>
                            </el-row>                            
                        </el-col>
                        <el-col :xs="24" :sm="6" :md="6" :lg="6">
                            <el-button type="primary">สมัครใช้ระบบฟรีตลอดไป</el-button>
                        </el-col>
                    </el-row>
                    <Package_list />
                </el-col>
            </el-row>
        </el-main>
        </el-container>
  </div>
</template>

<script>
import Package_list from './components/Package_list.vue'

export default {
  name: 'app',
  components: {
    Package_list
  }
}
</script>

<style lang="scss">
body, html {
    margin: 0;
    padding: 0;
}
#app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    margin: 0;
    padding: 0;
}

.m-navbar {
    background-color: white;
    color: red($color: #671cc9);
    height: 50px;
}

.m-content {
    padding: 30px;
    background-color: #efefef;
}

.m-subcontent {
    padding: 30px;
    background-color: #ffffff;
}

.image {
    width: 100%;
    height: 200px;
    background: #efefef;
    margin-bottom: 20px;
}

.m-side-detail {
    font-size: 18px;
}

.m-tag {
    background: #696969;
    color: #ffffff;
    border: none;
}


</style>
