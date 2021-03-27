<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>人员信息管理系统</title>
    <!-- 使用CDN引入vue和vue-resource组件 -->
    <script src="https://cdn.jsdelivr.net/npm/vue@2.5.16/dist/vue.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/vue-resource@1.5.2"></script>
    <link href="https://cdn.staticfile.org/twitter-bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
    <script></script>
</head>
<body>

    <div id="app">
        <!-- 对接口进行测试 -->
        <!-- <input type="button" value='测试接口' @click="testInterface('http://jsonplaceholder.typicode.com/users')"> -->

        <!-- 搜索栏 -->
        <div class="panel panel-primary">
              <div class="panel-heading">
                    <h3 class="panel-title">人员信息管理</h3>
              </div>
              <div class="panel-body" form-inline>
                    <label>按用户名搜索：
                        <input type="text" v-model='key' @keyup.enter="search(key)">
                    </label>
                    <label>
                        <input type="button" value='搜索' @click="search(key)">
                    </label>
              </div>
        </div>
        
        <!-- 人员列表栏 -->
        <!-- table-striped 	在 <tbody> 内添加斑马线形式的条纹 ( IE8 不支持) 
            table-hover 在 <tbody> 内的任一行启用鼠标悬停状态     -->
        <table class="table table-bordered table-hover  table-striped" v-if='detail == false'>
            <thead>
                <tr>
                    <th>ID</th>
                    <th>姓名</th>
                    <th>用户名</th>
                    <th>邮箱</th>
                    <th>手机</th>  
                    <th>公司名</th>
                    <th>详细</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for='item in list' :key='item.id'>
                    <td>{{ item.id }}</td>
                    <td>{{ item.name }}</td>
                    <td>{{ item.username }}</td>
                    <td>{{ item.email }}</td>
                    <td>{{ item.phone }}</td>
                    <td>{{ item.company.name }}</td>
                    <td>
                        <a href="" @click.prevent='moreinfo(item.id)'>点击查看详细信息</a>
                    </td>
                </tr>
            </tbody>
        </table>
        
        <div v-if='detail == true'>
            <table class="table table-bordered table-hover  table-striped" v-if='detail == true'>
                <thead>
                    <tr>
                        <th>姓名</th>
                        <th>用户名</th>
                        <th>邮箱</th>
                        <th>个人主页</th>
                        <th>手机</th>
                        <th>住址</th>
                        <th>邮编</th> 
                        <th>公司名</th>
    
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>{{ detailInfo.name }}</td>
                        <td>{{ detailInfo.username }}</td>
                        <td>{{ detailInfo.email }}</td>
                        <td>{{ detailInfo.website }}</td>
                        <td>{{ detailInfo.phone }}</td>
                        <td>{{ detailInfo.address.city }}&nbsp;{{ detailInfo.address.street }}</td>
                        <td>{{ detailInfo.address.zipcode }}</td>
                        <td>{{ detailInfo.company.name }}</td>
                    </tr>
                </tbody>
            </table>
            <input type="button" value='返回' @click="goBack">
        </div>
       
        
    </div>

    <script>
        var vm = new Vue({
            el: '#app',
            data: {
                list: [],
                key: '',
                detail: false,
                detailInfo: null
            },
            // 生命周期函数
            created() {
                this.getList()
            },
            // 生命周期函数
            updated() {
                console.log(this.key)
            },
            methods: {
                // 测试接口按钮
                testInterface(url){
                    this.$http.get(url).then((result) => {
                        console.log(result)
                        list1 = result.body
                        console.log(list1[0])
                    }).catch((err) => {
                        console.log('Error')
                    });
                },
                // 获取人员列表
                getList(){
                    this.$http.get('http://jsonplaceholder.typicode.com/users').then((result) => {
                        if(result.status == 200){
                            console.log('status ok');
                            this.list = result.body
                        }
                        else{
                            console.log('status error')
                        }
                    }).catch((err) => {
                        alert('获取数据失败')
                    });
                },
                // 按用户名搜索
                search(key){
                    var newList = [];
                    this.list.forEach(item => {
                        if(key != ''){
                            if(item.username.indexOf(key) != -1){
                                newList.push(item);
                                console.log(newList);
                                this.list = newList;
                            }
                        }
                        else{
                            this.getList();
                        }
                    });
                },
                // 显示用户具体信息
                moreinfo(id){
                    // this.detail = true;
                    this.detailInfo = this.list[id-1];
                    this.detail = !this.detail;
                    console.log(this.detailInfo);
                },
                goBack(){
                    this.detail = !this.detail;
                },
            }
        })
    </script>
</body>
</html>
