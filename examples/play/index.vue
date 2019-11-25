<template>
  <div style="margin: 20px;">
    <el-input v-model="input" placeholder="请输入内容"></el-input>
    <el-image
      v-for="(url, index) in list"
      :key="index"
      style="width: 80px; height: 80px"
      :src="url"
      :preview-src-list="list">
    </el-image>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        input: 'Hello Element UI!',
        list: ['https://cms-midea-test.oss-cn-hangzhou.aliyuncs.com/cmimp_beta/file/20191122/MswdQmp5YyBPXA6y',
        'https://cms-midea-test.oss-cn-hangzhou.aliyuncs.com/cmimp_beta/file/20191122/Gfz8JrEx5JF3wPnA',
        'https://cms-midea-test.oss-cn-hangzhou.aliyuncs.com/cmimp_beta/file/20191122/j5kNrJExeeffGMYE',
        'https://cms-midea-test.oss-cn-hangzhou.aliyuncs.com/cmimp_beta/file/20191122/bna6zY7iFYCAXfwC',
        'https://cms-midea-test.oss-cn-hangzhou.aliyuncs.com/cmimp_beta/file/20191122/WwRjj7t4XY6yXekY',
        'https://cms-midea-test.oss-cn-hangzhou.aliyuncs.com/cmimp_beta/file/20191122/cipQXPyJZ7cjRZXe']
      };
    }
  };
</script>
