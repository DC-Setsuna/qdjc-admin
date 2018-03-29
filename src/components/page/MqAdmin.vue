<template>
  <div class="mq-admin">
    <div class="crumbs">
      <el-breadcrumb separator="/">
        <el-breadcrumb-item><i class="el-icon-location"></i>MQ监控</el-breadcrumb-item>
        <el-breadcrumb-item>安全管理平台</el-breadcrumb-item>
      </el-breadcrumb>
    </div>
    <el-collapse>
      <el-collapse-item>
        <template slot="title">
          Local Queue Managers<i class="header-icon el-icon-info"></i>
        </template>
        <div style="padding-left: 20px;">
        	<table width="500" cellspacing="0" cellpadding="3">
        	<tr align="left" style="background-color:#eee;">
        		<th>Name</th>
        		<th>Status</th>
        	</tr>
        	<tr>
        		<td>DDXPQMGR</td>
        		<td style="color: #0cdb1e;"><i class="el-icon-loading"></i>Running</td>
        	</tr>
        	<tr>
        		<td>MDXPQMGR</td>
        		<td style="color: #0cdb1e;"><i class="el-icon-loading"></i>Running</td>
        	</tr>
        </table>
        </div>
        
      </el-collapse-item>
      <el-collapse-item title="Listeners 监听器">
        <div style="padding-left:20px;">
        	<table width="500" cellspacing="0" cellpadding="3">
        		<tr align="left" style="background-color:#eee;">
        			<th>Name</th>
        			<th>Port</th>
        			<th>Listener Status</th>
        		</tr>
        		<tr>
        			<td>LISTENER.TCP</td>
        			<td>1414</td>
        			<td style="color: #0cdb1e;"><i class="el-icon-loading"></i>Running</td>
        		</tr>
        	</table>
        </div>
      </el-collapse-item>
      <el-collapse-item title="Queens">
        <div style="padding-left:20px;">
        	<table width="500" cellspacing="0" cellpadding="3">
        		<tr align="left" style="background-color:#eee;">
        			<th>Queue Manager</th>
        			<th>Name</th>
        			<th>Type</th>
        			<th>Depth</th>
        		</tr>
        		<tr>
        			<td rowspan="2">DDXPQMGR</td>
        			<td>MDXP.INNER.REQUEST.INPUT</td>
        			<td>Local</td>
        			<td>20000</td>
        		</tr>
        		<tr>
        			<td>MDXP.INNER.REQUEST.OUTPUT</td>
        			<td>Local</td>
        			<td>10000</td>
        		</tr>
        		<tr>
        			<td rowspan="2">MDXPQMGR</td>
        			<td>MDXP.INNER.REQUEST.INPUT</td>
        			<td>Local</td>
        			<td>0</td>
        		</tr>
        		<tr>
        			<td>MDXP.INNER.REQUEST.OUTPUT</td>
        			<td>Remote</td>
        			<td>0</td>
        		</tr>
        	</table>
        </div>
      </el-collapse-item>
    </el-collapse>
  </div>
</template>
<script>
export default {
  data() {
    return {

    }
  }
}

</script>
<style>


</style>
