<template>    
    <el-date-picker
      v-model="valuetime"
      type="date"
      placeholder="选择日期">
    </el-date-picker>
</template>

<script>
    export default {
        data () {
            return {
                valuetime:'',
                }
            }
    }
</script>
