<template>
  <div class="ent_from">

    <div class="form_banner">
      <img src="../assets/images/form_banner.jpg" alt="">
      <p class="form_title">【心职】企业注册申请</p>
    </div>

    <div class="form_field">
      <p class="form_field_label">企业注册码</p>
      <input type="text" class="form_value_input" placeholder="企业注册后获得的六位随机数字">
    </div>

    <div class="form_field">
      <p class="form_field_label">企业名称</p>
      <input type="text" class="form_value_input" placeholder="如：宁波智士网络技术有限公司">
    </div>

    <div class="form_field">
      <p class="form_field_label">营业执照号码</p>
      <input type="text" class="form_value_input" placeholder="如：91330201316992528Q">
    </div>

    <div class="form_field">
     <!-- <p class="form_field_label01">公司对外简称 <br />-->
      <div class="form_field_label01">
        <p class="title_node">公司对外简称</p>
        <p class="field_note_fade">&nbsp 0/1~5</p>
      </div>
      <input type="text" class="form_value_input" placeholder="如：智士网络（1~5个字）">
    </div>

    <div class="form_field">
      <!-- <p class="form_field_label01">公司对外简称 <br />-->
      <div class="form_field_label01">
        <p class="title_node">企业地址</p>
        <p class="field_note_light">请填写真实地址，不然职位无法在地图上显示</p>
      </div>
      <div>
        <input type="text" class="form_input" placeholder="中国">
        <input type="text" class="form_input">
        <br />
        <input type="text" class="form_value_input01" placeholder="如：智士网络（1~5个字）">
      </div>
    </div>

    <div class="form_field">
      <p class="form_field_label">企业性质</p>
      <input type="text" class="form_value_input">
    </div>

    <div class="form_field">
      <p class="form_field_label">企业规模</p>
      <input type="text" class="form_value_input">
    </div>

    <div class="form_field">
      <!-- <p class="form_field_label01">公司对外简称 <br />-->
      <div class="form_field_label01">
        <p class="title_node">公司简介</p>
        <p class="field_note_fade">&nbsp 0/1~5</p>
      </div>
      <input type="text" class="form_value_input02" placeholder="企业介绍">
    </div>

    <div class="form_field">
      <div class="upload_field">
        <p class="form_field_label">企业LOGO图片</p>
        <p class="field_note_light">方形最佳</p>
        <p class="field_note_fade">支持 jpg,png,gif,bmp,psd,tiff等<br />图片格式</p>
      </div>
      <div class="upload_widget">
        <div class="upload_icon_set">
          <img src="../assets/images/upload_icon.png" alt="">
          <p>点击选择图片</p>
          <p>(需小于10M)</p>
        </div>
        <input type="file">
      </div>
    </div>

    <div class="form_field">
      <div class="upload_field">
        <p class="form_field_label">企业照片</p>
        <p class="field_note_fade">支持 jpg,png,gif,bmp,psd,tiff等<br />图片格式</p>
      </div>
      <div class="upload_widget">
        <div class="upload_icon_set">
          <img src="../assets/images/upload_icon.png" alt="">
          <p>点击选择图片</p>
          <p>(需小于10M)</p>
        </div>
        <input type="file">
      </div>
    </div>

    <div class="form_field">
      <p class="form_field_label">联系人姓名</p>
      <div class="insert_icon">
        <i class="input_icon name_icon"></i>
        <input type="text" class="form_value_input" placeholder="企业和心职平台的联系人">
      </div>
    </div>

    <div class="form_field">
      <p class="form_field_label">联系人手机</p>
      <div class="insert_icon">
        <i class="input_icon phone_icon"></i>
        <input type="text" class="form_value_input" placeholder="用于真实性核实">
      </div>
    </div>

    <div class="form_field">
      <p class="form_field_label">简历接收邮箱</p>
      <div class="insert_icon">
        <i class="input_icon email_icon"></i>
        <input type="text" class="form_value_input" placeholder="用于接收简历">
      </div>
    </div>

  </div>
</template>

<script>
  export default {
    name: "register01"
  }
</script>

<style scoped>

  .upload_field { /**上传图片备注容器**/
    width: 25%;
  }
  .upload_field .form_field_label{ /**单独设置上传图片字段容器宽度**/
    width: 100%;
  }
  .upload_widget{ /**上传图片空间总容器**/
    display: flex;
    align-items: center;
    width:150px;
    height: 150px;
    border: 1px dashed #999;
    background: #fff;
    cursor: pointer;
    position: relative;
    overflow: hidden;
    margin-left: 20px;
  }
  .upload_widget img{ /**上传图片控件图片**/
    width: 50%;
    height: auto;
    display: block;
    margin: 0 auto 10px auto;
  }
  .upload_widget input{ /**上传图片的控件按钮**/
    display: block;
    position: absolute;
    top:0;
    bottom: 0;
    right:0;
    left:0;
    opacity: 0;
    cursor: pointer;
  }
  .upload_icon_set p{ /**上传图片空间中的提示文字**/
    text-align: center;
    color: #999;
    font-size: 14px;
    line-height: 22px;
  }
  .company_icon::after {
    background: url("../assets/images/icon/building.png") no-repeat;
    background-size: 100% auto;
  }
</style>
