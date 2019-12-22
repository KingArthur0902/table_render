<template>
    <div>
        <div >table1</div>
        <table>
            <tbody>
            <tr v-for="item of tableList1">
                <td v-for="i of item" v-if="i !== undefined" :rowspan="i.rowspan && i.rowspan > 1 ? i.rowspan : 1">
                        <span v-if="i === undefined">
                            undifined
                        </span>
                    <span v-else>
                            {{i}}
                        </span>
                </td>
            </tr>
            </tbody>
        </table>
<!--        <table>
            <tbody>
            <tr v-for="item of tableList3">
                <td v-for="i of item" >
                        <span v-if="i === undefined">
                            undifined
                        </span>
                    <span v-else>
                            {{i}}
                        </span>
                </td>
            </tr>
            </tbody>
        </table>-->

        <br/>
        <div >table2</div>
        <table>
            <tbody>
            <tr v-for="item of tableList2">
                <td v-for="i of item" v-if="i !== undefined" :rowspan="i.rowspan && i.rowspan > 1 ? i.rowspan : 1" :colspan="i.colspan && i.colspan > 1 ? i.colspan : 1">
                        <span v-if="i === undefined">
                            undifined
                        </span>
                    <span v-else>
                            {{i}}
                        </span>
                </td>
            </tr>
            </tbody>
        </table>
        <br/>
        <div >table3</div>
        <table>
            <tbody>
            <tr v-for="item of tableList3">
                <td v-for="i of item" v-if="i !== undefined" :rowspan="i.rowspan && i.rowspan > 1 ? i.rowspan : 1" :colspan="i.colspan && i.colspan > 1 ? i.colspan : 1">
                        <span v-if="i === undefined">
                            undifined
                        </span>
                    <span v-else>
                            {{i}}
                        </span>
                </td>
            </tr>
            </tbody>
        </table>
        <br/>
        <div >table4</div>
        <table>
            <tbody>
            <tr v-for="item of tableList4">
                <td v-for="i of item" v-if="i !== undefined" :rowspan="i.rowspan && i.rowspan > 1 ? i.rowspan : 1" :colspan="i.colspan && i.colspan > 1 ? i.colspan : 1">
                        <span v-if="i === undefined">
                            undifined
                        </span>
                    <span v-else>
                            {{i}}
                        </span>
                </td>
            </tr>
            </tbody>
        </table>
        <br/>
        <div >table5</div>
        <table>
            <tbody>
            <tr v-for="item of tableList5">
                <td v-for="i of item" v-if="i !== undefined" :rowspan="i.rowspan && i.rowspan > 1 ? i.rowspan : 1" :colspan="i.colspan && i.colspan > 1 ? i.colspan : 1">
                        <span v-if="i === undefined">
                            undifined
                        </span>
                    <span v-else>
                            {{i}}
                        </span>
                </td>
            </tr>
            </tbody>
        </table>
        <br/>
        <div >table6</div>
        <table>
            <tbody>
            <tr v-for="item of tableList6">
                <td v-for="i of item" v-if="i !== undefined" :rowspan="i.rowspan && i.rowspan > 1 ? i.rowspan : 1" :colspan="i.colspan && i.colspan > 1 ? i.colspan : 1">
                        <span v-if="i === undefined">
                            undifined
                        </span>
                    <span v-else>
                            {{i}}
                        </span>
                </td>
            </tr>
            </tbody>
        </table>
        <br/>
        <div >table7</div>
        <table>
            <tbody>
            <tr v-for="item of tableList7">
                <td v-for="i of item" v-if="i !== undefined" :rowspan="i.rowspan && i.rowspan > 1 ? i.rowspan : 1" :colspan="i.colspan && i.colspan > 1 ? i.colspan : 1">
                        <span v-if="i === undefined">
                            undifined
                        </span>
                    <span v-else>
                            {{i}}
                        </span>
                </td>
            </tr>
            </tbody>
        </table>

        <br/>
        <div >table8</div>
        <table>
            <tbody>
            <tr v-for="item of tableList8">
                <td v-for="i of item" v-if="i !== undefined" :rowspan="i.rowspan && i.rowspan > 1 ? i.rowspan : 1" :colspan="i.colspan && i.colspan > 1 ? i.colspan : 1">
                        <span v-if="i === undefined">
                            undifined
                        </span>
                    <span v-else>
                            {{i}}
                        </span>
                </td>
            </tr>
            </tbody>
        </table>

        <br/>
        <div >table9</div>
        <table>
            <tbody>
            <tr v-for="item of tableList9">
                <td v-for="i of item" v-if="i !== undefined" :rowspan="i.rowspan && i.rowspan > 1 ? i.rowspan : 1" :colspan="i.colspan && i.colspan > 1 ? i.colspan : 1">
                        <span v-if="i === undefined">
                            undifined
                        </span>
                    <span v-else>
                            {{i}}
                        </span>
                </td>
            </tr>
            </tbody>
        </table>
    </div>
</template>

<script>
    export default {
        name: "MyTable",
        data() {
            return {
                tableList1: [],
                tableList2:[],
                tableList3:[],
                tableList4: [],
                tableList5:[],
                tableList6:[],
                tableList7: [],
                tableList8:[],
                tableList9:[]
            }
        },
        created() {
            let dataConfig = {
                "rows": [{
                    "columnName": "area",
                    "alias": "区",
                    "filterType": "eq",
                    "values": [],
                    "id": "zsuuvzmp3joanbjeepvmj4xe6bggp57t"
                }, {
                    "columnName": "year",
                    "alias": "年",
                    "filterType": "eq",
                    "values": [],
                    "id": "lnfovnxah3yqvnkn6s4grhu8fpa1rzio"
                }, {
                    "columnName": "age_group",
                    "alias": "分组类型",
                    "filterType": "eq",
                    "values": [],
                    "id": "ldznt1stolnkwbtmr13l1hns6fa9mkzg"
                }],
                "columns": [{
                    "columnName": "audit_state",
                    "alias": "审核状态",
                    "filterType": "eq",
                    "values": [],
                    "id": "ptdnrxnj2bwbrkjsmhxu2d3lc4437dzq"
                }],
                "filters": [],
                "values": [{"column": "male_num", "alias": "男性人口数", "aggType": "max"}]
            }
            let dataList = {
                "columnList": [{"index": 0, "aggType": null, "name": "audit_state", "alias": "审核状态"}, {
                    "index": 1,
                    "aggType": null,
                    "name": "area",
                    "alias": "区"
                }, {"index": 2, "aggType": null, "name": "year", "alias": "年"}, {
                    "index": 3,
                    "aggType": null,
                    "name": "age_group",
                    "alias": "分组类型"
                }, {"index": 4, "aggType": "max", "name": "male_num", "alias": "男性人口数"}],
                "data": [["二审通过", "海珠区", "2017", "0-", "3583"], ["二审通过", "海珠区", "2017", "1-", "4374"], ["二审通过", "海珠区", "2017", "10-", "12005"], ["二审通过", "海珠区", "2017", "15-", "13684"], ["二审通过", "海珠区", "2017", "2-", "3601"], ["二审通过", "海珠区", "2017", "20-", "17763"], ["二审通过", "海珠区", "2017", "25-", "24709"], ["二审通过", "海珠区", "2017", "3-", "3445"], ["二审通过", "海珠区", "2017", "30-", "28049"], ["二审通过", "海珠区", "2017", "35-", "23709"], ["二审通过", "海珠区", "2017", "4-", "3186"], ["二审通过", "海珠区", "2017", "40-", "21619"], ["二审通过", "海珠区", "2017", "45-", "27491"], ["二审通过", "海珠区", "2017", "5-", "3571"], ["二审通过", "海珠区", "2017", "50-", "31039"], ["二审通过", "海珠区", "2017", "55-", "36632"], ["二审通过", "海珠区", "2017", "6-", "2891"], ["二审通过", "海珠区", "2017", "60-", "35177"], ["二审通过", "海珠区", "2017", "65-", "22168"], ["二审通过", "海珠区", "2017", "7-", "2742"], ["二审通过", "海珠区", "2017", "70-", "13201"], ["二审通过", "海珠区", "2017", "75-", "9233"], ["二审通过", "海珠区", "2017", "8-", "2380"], ["二审通过", "海珠区", "2017", "80-", "7831"], ["二审通过", "海珠区", "2017", "85及以上", "5878"], ["二审通过", "海珠区", "2017", "9-", "2673"], ["二审通过", "海珠区", "2017", "合计", "362634"], ["二审通过", "荔湾区", "2017", "0-", "5298"], ["二审通过", "荔湾区", "2017", "1-", "6811"], ["二审通过", "荔湾区", "2017", "10-", "21687"], ["二审通过", "荔湾区", "2017", "15-", "23418"], ["二审通过", "荔湾区", "2017", "2-", "5593"], ["二审通过", "荔湾区", "2017", "20-", "29272"], ["二审通过", "荔湾区", "2017", "25-", "43290"], ["二审通过", "荔湾区", "2017", "3-", "5293"], ["二审通过", "荔湾区", "2017", "30-", "43008"], ["二审通过", "荔湾区", "2017", "35-", "40950"], ["二审通过", "荔湾区", "2017", "4-", "5086"], ["二审通过", "荔湾区", "2017", "40-", "38773"], ["二审通过", "荔湾区", "2017", "45-", "48990"], ["二审通过", "荔湾区", "2017", "5-", "5944"], ["二审通过", "荔湾区", "2017", "50-", "49338"], ["二审通过", "荔湾区", "2017", "55-", "49918"], ["二审通过", "荔湾区", "2017", "6-", "5273"], ["二审通过", "荔湾区", "2017", "60-", "48045"], ["二审通过", "荔湾区", "2017", "65-", "32205"], ["二审通过", "荔湾区", "2017", "7-", "4980"], ["二审通过", "荔湾区", "2017", "70-", "18307"], ["二审通过", "荔湾区", "2017", "75-", "14869"], ["二审通过", "荔湾区", "2017", "8-", "4513"], ["二审通过", "荔湾区", "2017", "80-", "13666"], ["二审通过", "荔湾区", "2017", "85及以上", "10357"], ["二审通过", "荔湾区", "2017", "9-", "5067"], ["二审通过", "荔湾区", "2017", "合计", "579951"], ["未提交审核", "荔湾区", "2017", "0-", "3583"], ["未提交审核", "荔湾区", "2017", "1-", "4374"], ["未提交审核", "荔湾区", "2017", "10-", "12005"], ["未提交审核", "荔湾区", "2017", "15-", "13684"], ["未提交审核", "荔湾区", "2017", "2-", "3601"], ["未提交审核", "荔湾区", "2017", "20-", "17763"], ["未提交审核", "荔湾区", "2017", "25-", "24709"], ["未提交审核", "荔湾区", "2017", "3-", "3445"], ["未提交审核", "荔湾区", "2017", "30-", "28049"], ["未提交审核", "荔湾区", "2017", "35-", "23709"], ["未提交审核", "荔湾区", "2017", "4-", "3186"], ["未提交审核", "荔湾区", "2017", "40-", "21619"], ["未提交审核", "荔湾区", "2017", "45-", "27491"], ["未提交审核", "荔湾区", "2017", "5-", "3571"], ["未提交审核", "荔湾区", "2017", "50-", "31039"], ["未提交审核", "荔湾区", "2017", "55-", "36632"], ["未提交审核", "荔湾区", "2017", "6-", "2891"], ["未提交审核", "荔湾区", "2017", "60-", "35177"], ["未提交审核", "荔湾区", "2017", "65-", "22168"], ["未提交审核", "荔湾区", "2017", "7-", "2742"], ["未提交审核", "荔湾区", "2017", "70-", "13201"], ["未提交审核", "荔湾区", "2017", "75-", null], ["未提交审核", "荔湾区", "2017", "8-", "2380"], ["未提交审核", "荔湾区", "2017", "80-", "7831"], ["未提交审核", "荔湾区", "2017", "85及以上", "5878"], ["未提交审核", "荔湾区", "2017", "9-", "2673"], ["未提交审核", "荔湾区", "2017", "合计", "362634"]]
            }
            let rows = dataConfig.rows.map(op => {
                return op.columnName
            })
            let columns = dataConfig.columns.map(op => {
                return op.columnName
            })
            let values = dataConfig.values.map(op => {
                return op.column
            })

            this.tableList1 = this.convertToTable(dataList, rows, columns, values);
            this.tableList2 = this.convertToTable(dataList, [], columns, values);
            this.tableList3 = this.convertToTable(dataList, rows, [], values);


            let dataConfig2 = {"rows":[{"columnName":"age_group","alias":"分组类型","filterType":"eq","values":[],"id":"ldznt1stolnkwbtmr13l1hns6fa9mkzg"},{"columnName":"area","alias":"区","filterType":"eq","values":[],"id":"zsuuvzmp3joanbjeepvmj4xe6bggp57t"},{"columnName":"audit_state","alias":"审核状态","filterType":"eq","values":[],"id":"ptdnrxnj2bwbrkjsmhxu2d3lc4437dzq"}],"columns":[{"columnName":"year","alias":"年","filterType":"eq","values":[],"id":"lnfovnxah3yqvnkn6s4grhu8fpa1rzio"}],"filters":[],"values":[{"column":"male_num","alias":"男性人口数","aggType":"max"},{"column":"female_num","alias":"女性人口数","aggType":"avg"}]}

            let rows2 = dataConfig2.rows.map(op => {
                return op.columnName
            })
            let columns2 = dataConfig2.columns.map(op => {
                return op.columnName
            })
            let values2 = dataConfig2.values.map(op => {
                return op.column
            })


            let dataList2 = {"columnList":[{"index":0,"aggType":null,"name":"year","alias":"年"},{"index":1,"aggType":null,"name":"age_group","alias":"分组类型"},{"index":2,"aggType":null,"name":"area","alias":"区"},{"index":3,"aggType":null,"name":"audit_state","alias":"审核状态"},{"index":4,"aggType":"max","name":"male_num","alias":"男性人口数"},{"index":5,"aggType":"avg","name":"female_num","alias":"女性人口数"}],"data":[["2017","0-","海珠区","二审通过","3583","3199.0000"],["2017","0-","荔湾区","二审通过","5298","3929.0000"],["2017","0-","荔湾区","未提交审核","3583","3199.0000"],["2017","1-","海珠区","二审通过","4374","3804.0000"],["2017","1-","荔湾区","二审通过","6811","5039.5000"],["2017","1-","荔湾区","未提交审核","4374","3804.0000"],["2017","10-","海珠区","二审通过","12005","11069.0000"],["2017","10-","荔湾区","二审通过","21687","15286.5000"],["2017","10-","荔湾区","未提交审核","12005","11069.0000"],["2017","15-","海珠区","二审通过","13684","12361.0000"],["2017","15-","荔湾区","二审通过","23418","16840.5000"],["2017","15-","荔湾区","未提交审核","13684","12361.0000"],["2017","2-","海珠区","二审通过","3601","3351.0000"],["2017","2-","荔湾区","二审通过","5593","4198.5000"],["2017","2-","荔湾区","未提交审核","3601","3351.0000"],["2017","20-","海珠区","二审通过","17763","16634.0000"],["2017","20-","荔湾区","二审通过","29272","22717.5000"],["2017","20-","荔湾区","未提交审核","17763","16634.0000"],["2017","25-","海珠区","二审通过","24709","24029.0000"],["2017","25-","荔湾区","二审通过","43290","33390.5000"],["2017","25-","荔湾区","未提交审核","24709","24029.0000"],["2017","3-","海珠区","二审通过","3445","3048.0000"],["2017","3-","荔湾区","二审通过","5293","3874.5000"],["2017","3-","荔湾区","未提交审核","3445","3048.0000"],["2017","30-","海珠区","二审通过","28049","28389.0000"],["2017","30-","荔湾区","二审通过","43008","36775.5000"],["2017","30-","荔湾区","未提交审核","28049","28389.0000"],["2017","35-","海珠区","二审通过","23709","25478.0000"],["2017","35-","荔湾区","二审通过","40950","36472.0000"],["2017","35-","荔湾区","未提交审核","23709","25478.0000"],["2017","4-","海珠区","二审通过","3186","2817.0000"],["2017","4-","荔湾区","二审通过","5086","3741.5000"],["2017","4-","荔湾区","未提交审核","3186","2817.0000"],["2017","40-","海珠区","二审通过","21619","23916.0000"],["2017","40-","荔湾区","二审通过","38773","34093.0000"],["2017","40-","荔湾区","未提交审核","21619","23916.0000"],["2017","45-","海珠区","二审通过","27491","30807.0000"],["2017","45-","荔湾区","二审通过","48990","41915.5000"],["2017","45-","荔湾区","未提交审核","27491","30807.0000"],["2017","5-","海珠区","二审通过","3571","3186.0000"],["2017","5-","荔湾区","二审通过","5944","4230.5000"],["2017","5-","荔湾区","未提交审核","3571","3186.0000"],["2017","50-","海珠区","二审通过","31039","32522.0000"],["2017","50-","荔湾区","二审通过","49338","40097.0000"],["2017","50-","荔湾区","未提交审核","31039","32522.0000"],["2017","55-","海珠区","二审通过","36632","35496.0000"],["2017","55-","荔湾区","二审通过","49918","41973.5000"],["2017","55-","荔湾区","未提交审核","36632","35496.0000"],["2017","6-","海珠区","二审通过","2891","2706.0000"],["2017","6-","荔湾区","二审通过","5273","3616.5000"],["2017","6-","荔湾区","未提交审核","2891","2706.0000"],["2017","60-","海珠区","二审通过","35177","34503.0000"],["2017","60-","荔湾区","二审通过","48045","42151.5000"],["2017","60-","荔湾区","未提交审核","35177","34503.0000"],["2017","65-","海珠区","二审通过","22168","22228.0000"],["2017","65-","荔湾区","二审通过","32205","26504.5000"],["2017","65-","荔湾区","未提交审核","22168","22228.0000"],["2017","7-","海珠区","二审通过","2742","2450.0000"],["2017","7-","荔湾区","二审通过","4980","3427.5000"],["2017","7-","荔湾区","未提交审核","2742","2450.0000"],["2017","70-","海珠区","二审通过","13201","13430.0000"],["2017","70-","荔湾区","二审通过","18307","16777.5000"],["2017","70-","荔湾区","未提交审核","13201",null],["2017","75-","海珠区","二审通过","9233","11144.0000"],["2017","75-","荔湾区","二审通过","14869","14545.0000"],["2017","75-","荔湾区","未提交审核",null,"11144.0000"],["2017","8-","海珠区","二审通过","2380","2197.0000"],["2017","8-","荔湾区","二审通过","4513","3150.5000"],["2017","8-","荔湾区","未提交审核","2380","2197.0000"],["2017","80-","海珠区","二审通过","7831","12304.0000"],["2017","80-","荔湾区","二审通过","13666","15588.5000"],["2017","80-","荔湾区","未提交审核","7831","12304.0000"],["2017","85及以上","海珠区","二审通过","5878","9848.0000"],["2017","85及以上","荔湾区","二审通过","10357","11954.5000"],["2017","85及以上","荔湾区","未提交审核","5878","9848.0000"],["2017","9-","海珠区","二审通过","2673","2389.0000"],["2017","9-","荔湾区","二审通过","5067","3500.5000"],["2017","9-","荔湾区","未提交审核","2673","2389.0000"],["2017","合计","海珠区","二审通过","362634","373305.0000"],["2017","合计","荔湾区","二审通过","579951","485791.5000"],["2017","合计","荔湾区","未提交审核","362634","373305.0000"]]}
            this.tableList4 = this.convertToTable(dataList2, rows2, columns2, values2);
            this.tableList5 = this.convertToTable(dataList2, [], columns2, values2);
            this.tableList6 = this.convertToTable(dataList2, rows2, [], values2);


            let dataConfig3 = {"rows":[{"columnName":"age_group","alias":"分组类型","filterType":"eq","values":[],"id":"ldznt1stolnkwbtmr13l1hns6fa9mkzg"},{"columnName":"update_date","alias":"更新日期","filterType":"eq","values":[],"id":"8eqsa23izfjf7m8ibhvvp21vugi2oo7l"},{"columnName":"year","alias":"年","filterType":"eq","values":[],"id":"lnfovnxah3yqvnkn6s4grhu8fpa1rzio"},{"columnName":"audit_state","alias":"审核状态","filterType":"eq","values":[],"id":"ptdnrxnj2bwbrkjsmhxu2d3lc4437dzq"}],"columns":[{"columnName":"area","alias":"区","filterType":"eq","values":[],"id":"zsuuvzmp3joanbjeepvmj4xe6bggp57t"}],"filters":[],"values":[{"column":"male_num","alias":"男性人口数","aggType":"max"},{"column":"female_num","alias":"女性人口数","aggType":"avg"}]}

            let rows3 = dataConfig3.rows.map(op => {
                return op.columnName
            })
            let columns3 = dataConfig3.columns.map(op => {
                return op.columnName
            })
            let values3 = dataConfig3.values.map(op => {
                return op.column
            })
            let dataList3 = {"columnList":[{"index":0,"aggType":null,"name":"area","alias":"区"},{"index":1,"aggType":null,"name":"age_group","alias":"分组类型"},{"index":2,"aggType":null,"name":"update_date","alias":"更新日期"},{"index":3,"aggType":null,"name":"year","alias":"年"},{"index":4,"aggType":null,"name":"audit_state","alias":"审核状态"},{"index":5,"aggType":"max","name":"male_num","alias":"男性人口数"},{"index":6,"aggType":"avg","name":"female_num","alias":"女性人口数"}],"data":[["海珠区","0-","2019-11-25","2017","二审通过","3583","3199.0000"],["海珠区","1-","2019-11-25","2017","二审通过","4374","3804.0000"],["海珠区","10-","2019-11-25","2017","二审通过","12005","11069.0000"],["海珠区","15-","2019-11-25","2017","二审通过","13684","12361.0000"],["海珠区","2-","2019-11-25","2017","二审通过","3601","3351.0000"],["海珠区","20-","2019-11-25","2017","二审通过","17763","16634.0000"],["海珠区","25-","2019-11-25","2017","二审通过","24709","24029.0000"],["海珠区","3-","2019-11-25","2017","二审通过","3445","3048.0000"],["海珠区","30-","2019-11-25","2017","二审通过","28049","28389.0000"],["海珠区","35-","2019-11-25","2017","二审通过","23709","25478.0000"],["海珠区","4-","2019-11-25","2017","二审通过","3186","2817.0000"],["海珠区","40-","2019-11-25","2017","二审通过","21619","23916.0000"],["海珠区","45-","2019-11-25","2017","二审通过","27491","30807.0000"],["海珠区","5-","2019-11-25","2017","二审通过","3571","3186.0000"],["海珠区","50-","2019-11-25","2017","二审通过","31039","32522.0000"],["海珠区","55-","2019-11-25","2017","二审通过","36632","35496.0000"],["海珠区","6-","2019-11-25","2017","二审通过","2891","2706.0000"],["海珠区","60-","2019-11-25","2017","二审通过","35177","34503.0000"],["海珠区","65-","2019-11-25","2017","二审通过","22168","22228.0000"],["海珠区","7-","2019-11-25","2017","二审通过","2742","2450.0000"],["海珠区","70-","2019-11-25","2017","二审通过","13201","13430.0000"],["海珠区","75-","2019-11-25","2017","二审通过","9233","11144.0000"],["海珠区","8-","2019-11-25","2017","二审通过","2380","2197.0000"],["海珠区","80-","2019-11-25","2017","二审通过","7831","12304.0000"],["海珠区","85及以上","2019-11-25","2017","二审通过","5878","9848.0000"],["海珠区","9-","2019-11-25","2017","二审通过","2673","2389.0000"],["海珠区","合计","2019-11-25","2017","二审通过","362634","373305.0000"],["荔湾区","0-","#NULL","2017","未提交审核","3583","3199.0000"],["荔湾区","0-","2019-11-22","2017","二审通过","3583","3199.0000"],["荔湾区","0-","2019-11-25","2017","二审通过","5298","4659.0000"],["荔湾区","1-","#NULL","2017","未提交审核","4374","3804.0000"],["荔湾区","1-","2019-11-22","2017","二审通过","4374","3804.0000"],["荔湾区","1-","2019-11-25","2017","二审通过","6811","6275.0000"],["荔湾区","10-","#NULL","2017","未提交审核","12005","11069.0000"],["荔湾区","10-","2019-11-22","2017","二审通过","12005","11069.0000"],["荔湾区","10-","2019-11-25","2017","二审通过","21687","19504.0000"],["荔湾区","15-","#NULL","2017","未提交审核","13684","12361.0000"],["荔湾区","15-","2019-11-22","2017","二审通过","13684","12361.0000"],["荔湾区","15-","2019-11-25","2017","二审通过","23418","21320.0000"],["荔湾区","2-","#NULL","2017","未提交审核","3601","3351.0000"],["荔湾区","2-","2019-11-22","2017","二审通过","3601","3351.0000"],["荔湾区","2-","2019-11-25","2017","二审通过","5593","5046.0000"],["荔湾区","20-","#NULL","2017","未提交审核","17763","16634.0000"],["荔湾区","20-","2019-11-22","2017","二审通过","17763","16634.0000"],["荔湾区","20-","2019-11-25","2017","二审通过","29272","28801.0000"],["荔湾区","25-","#NULL","2017","未提交审核","24709","24029.0000"],["荔湾区","25-","2019-11-22","2017","二审通过","24709","24029.0000"],["荔湾区","25-","2019-11-25","2017","二审通过","43290","42752.0000"],["荔湾区","3-","#NULL","2017","未提交审核","3445","3048.0000"],["荔湾区","3-","2019-11-22","2017","二审通过","3445","3048.0000"],["荔湾区","3-","2019-11-25","2017","二审通过","5293","4701.0000"],["荔湾区","30-","#NULL","2017","未提交审核","28049","28389.0000"],["荔湾区","30-","2019-11-22","2017","二审通过","28049","28389.0000"],["荔湾区","30-","2019-11-25","2017","二审通过","43008","45162.0000"],["荔湾区","35-","#NULL","2017","未提交审核","23709","25478.0000"],["荔湾区","35-","2019-11-22","2017","二审通过","23709","25478.0000"],["荔湾区","35-","2019-11-25","2017","二审通过","40950","47466.0000"],["荔湾区","4-","#NULL","2017","未提交审核","3186","2817.0000"],["荔湾区","4-","2019-11-22","2017","二审通过","3186","2817.0000"],["荔湾区","4-","2019-11-25","2017","二审通过","5086","4666.0000"],["荔湾区","40-","#NULL","2017","未提交审核","21619","23916.0000"],["荔湾区","40-","2019-11-22","2017","二审通过","21619","23916.0000"],["荔湾区","40-","2019-11-25","2017","二审通过","38773","44270.0000"],["荔湾区","45-","#NULL","2017","未提交审核","27491","30807.0000"],["荔湾区","45-","2019-11-22","2017","二审通过","27491","30807.0000"],["荔湾区","45-","2019-11-25","2017","二审通过","48990","53024.0000"],["荔湾区","5-","#NULL","2017","未提交审核","3571","3186.0000"],["荔湾区","5-","2019-11-22","2017","二审通过","3571","3186.0000"],["荔湾区","5-","2019-11-25","2017","二审通过","5944","5275.0000"],["荔湾区","50-","#NULL","2017","未提交审核","31039","32522.0000"],["荔湾区","50-","2019-11-22","2017","二审通过","31039","32522.0000"],["荔湾区","50-","2019-11-25","2017","二审通过","49338","47672.0000"],["荔湾区","55-","#NULL","2017","未提交审核","36632","35496.0000"],["荔湾区","55-","2019-11-22","2017","二审通过","36632","35496.0000"],["荔湾区","55-","2019-11-25","2017","二审通过","49918","48451.0000"],["荔湾区","6-","#NULL","2017","未提交审核","2891","2706.0000"],["荔湾区","6-","2019-11-22","2017","二审通过","2891","2706.0000"],["荔湾区","6-","2019-11-25","2017","二审通过","5273","4527.0000"],["荔湾区","60-","#NULL","2017","未提交审核","35177","34503.0000"],["荔湾区","60-","2019-11-22","2017","二审通过","35177","34503.0000"],["荔湾区","60-","2019-11-25","2017","二审通过","48045","49800.0000"],["荔湾区","65-","#NULL","2017","未提交审核","22168","22228.0000"],["荔湾区","65-","2019-11-22","2017","二审通过","22168","22228.0000"],["荔湾区","65-","2019-11-25","2017","二审通过","32205","30781.0000"],["荔湾区","7-","#NULL","2017","未提交审核","2742","2450.0000"],["荔湾区","7-","2019-11-22","2017","二审通过","2742","2450.0000"],["荔湾区","7-","2019-11-25","2017","二审通过","4980","4405.0000"],["荔湾区","70-","#NULL","2017","未提交审核","13201",null],["荔湾区","70-","2019-11-22","2017","二审通过","13201","13430.0000"],["荔湾区","70-","2019-11-25","2017","二审通过","18307","20125.0000"],["荔湾区","75-","#NULL","2017","未提交审核",null,"11144.0000"],["荔湾区","75-","2019-11-22","2017","二审通过","9233","11144.0000"],["荔湾区","75-","2019-11-25","2017","二审通过","14869","17946.0000"],["荔湾区","8-","#NULL","2017","未提交审核","2380","2197.0000"],["荔湾区","8-","2019-11-22","2017","二审通过","2380","2197.0000"],["荔湾区","8-","2019-11-25","2017","二审通过","4513","4104.0000"],["荔湾区","80-","#NULL","2017","未提交审核","7831","12304.0000"],["荔湾区","80-","2019-11-22","2017","二审通过","7831","12304.0000"],["荔湾区","80-","2019-11-25","2017","二审通过","13666","18873.0000"],["荔湾区","85及以上","#NULL","2017","未提交审核","5878","9848.0000"],["荔湾区","85及以上","2019-11-22","2017","二审通过","5878","9848.0000"],["荔湾区","85及以上","2019-11-25","2017","二审通过","10357","14061.0000"],["荔湾区","9-","#NULL","2017","未提交审核","2673","2389.0000"],["荔湾区","9-","2019-11-22","2017","二审通过","2673","2389.0000"],["荔湾区","9-","2019-11-25","2017","二审通过","5067","4612.0000"],["荔湾区","合计","#NULL","2017","未提交审核","362634","373305.0000"],["荔湾区","合计","2019-11-22","2017","二审通过","362634","373305.0000"],["荔湾区","合计","2019-11-25","2017","二审通过","579951","598278.0000"]]}
            this.tableList7 = this.convertToTable(dataList3, rows3, columns3, values3);
            this.tableList8 = this.convertToTable(dataList3, [], columns3, values3);
            this.tableList9 = this.convertToTable(dataList3, rows3, [], values3);

            for (let d of dataList3.data) {
                for (let a of d) {
                    if (a === '0-') {
                       // console.log(d)
                    }
                }
            }
        },
        methods: {
            convertToTable(dataList, rows, columns, values) {
                let columnIndexMap = new Map();
                for (let c of dataList.columnList) {
                    columnIndexMap.set(c.name, c);
                }
                let data = dataList.data;

                let tableMap = new Map();
                let rowTitleMap = new Map();
                let columnTitleMap = new Map();

                function check(d, arrs, titleMap) {
                    let key = ''
                    let i = 0;
                    let map = titleMap;
                    for (let arr of arrs) {
                        let c = columnIndexMap.get(arr);
                        let index = c.index;
                        let k = d[index];
                        if (i > 0) {
                            key += '_';
                        }
                        key += k;
                        i++;
                        let childMap = map.get(k);
                        if (childMap === null || childMap === undefined) {
                            childMap = new Map();
                            map.set(k, childMap);
                        }
                        map = childMap;
                    }
                    return key;
                }

                for (let d of data) {

                    let trKey = check(d, rows, rowTitleMap);
                    let tdKey = check(d, columns, columnTitleMap);

                    let trMap = tableMap.get(trKey);

                    if (trMap === null || trMap === undefined) {
                        trMap = new Map();
                        tableMap.set(trKey, trMap);
                    }

                    let tdMap = trMap.get(tdKey);
                    if (tdMap === null || tdMap === undefined) {
                        tdMap = new Map();
                        trMap.set(tdKey, tdMap);
                    }

                    for (let v of values) {
                        let c = columnIndexMap.get(v);
                        let index = c.index;
                        let _v = d[index] || 0;

                        let existCount = tdMap.get(v) || 0;
                        tdMap.set(v, Number(_v) + Number(existCount));
                    }
                }

                function getTitles(spanName, trs, titleArr, map, pre, index) {
                    if (pre === null || pre === undefined) {
                        pre = '';
                    }
                    if (index === null || index === undefined) {
                        index = 0;
                    }
                    let tr = trs[index];
                    let totalC = 0;
                    for (let [k, v] of map.entries()) {
                        let o = {name:k}
                        if (v === null || v === undefined || v.size === 0) {
                            titleArr.push(pre + k);
                            let c = spanName === 'colspan' ? values.length :1 ;
                            o[spanName] = c;
                            totalC += c;
                            tr.push(o)
                        } else {
                            let c = getTitles(spanName, trs, titleArr, v, pre + k + '_', index + 1);
                            totalC +=c;
                            o[spanName] = c;
                            tr.push(o);
                        }
                    }
                    return totalC;
                }

                let rowTitleArr = [];
                let columnTitleArr = []

                let rowTitleTrs = [];
                let columnTitleTrs = [];

                for (let i = 0; i < rows.length; i++) {
                    let a = [];

                    rowTitleTrs.push(a);
                }
                for (let i = 0; i < columns.length; i++) {
                    let a = [];
                    for (let j = 0; j < rows.length; j++) {
                        a.push({});
                    }
                    columnTitleTrs.push(a);
                }

                getTitles('rowspan', rowTitleTrs, rowTitleArr, rowTitleMap);
                getTitles('colspan', columnTitleTrs, columnTitleArr, columnTitleMap);

                function patchEmpty(arr,spanName) {
                    if (arr === null || arr === undefined || arr.length === 0) {
                        return;
                    }
                    let _arr =[];
                    for (let a of arr) {
                        _arr.push(a);
                        if (a && a[spanName] && a[spanName] > 1) {
                            for (let j = 0; j < a[spanName] - 1; j++) {
                                _arr.push(undefined)
                            }
                        }
                    }

                    return _arr;
                }
                let l = rowTitleTrs.length;
                for (let i = 0; i<  l; i++) {
                    let arr= patchEmpty(rowTitleTrs[i], 'rowspan');
                    rowTitleTrs[i] = arr;
                }
                l = columnTitleTrs.length;

                for (let i = 0; i<  l; i++) {
                    let arr =  patchEmpty(columnTitleTrs[i],'colspan');
                    columnTitleTrs[i] = arr;
                }

                let convertedRowTitleTrs = new Map();

                for (let i = 0; i < rowTitleArr.length; i++) {
                    let arr = [];
                    for (let a of rowTitleTrs) {
                        arr.push(a[i]);
                    }
                    convertedRowTitleTrs.set(rowTitleArr[i], arr);
                }

                let table = [];

                if (rowTitleArr.length === 0) {
                    rowTitleArr.push('')
                }
                for (let trKey of rowTitleArr) {
                    let trMap = tableMap.get(trKey);
                    let tr = convertedRowTitleTrs.get(trKey) || [];
                    if (columnTitleArr && columnTitleArr.length > 0) {
                        for (let columnKey of columnTitleArr) {
                            let td = trMap.get(columnKey);
                            if (td === null || td === undefined) {
                                for (let j = 0; j < values.length; j++) {
                                    tr.push(0);
                                }
                            } else {
                                for (let v of values) {
                                    tr.push(td.get(v));
                                }
                            }
                        }
                    }else{
                        let td = trMap.get('');
                        if (td === null || td === undefined) {
                            for (let j = 0; j < values.length; j++) {
                                tr.push(0);
                            }
                        } else {
                            for (let v of values) {
                                tr.push(td.get(v));
                            }
                        }
                    }

                    table.push(tr);
                }

                let resultName = [];

                for (let a of rows) {
                    resultName.push(a);
                }
                if (columnTitleArr && columnTitleArr.length > 0) {
                    for (let a of columnTitleArr) {
                        for (let v of values) {
                            resultName.push(v);
                        }
                    }
                }else{
                    for (let v of values) {
                        resultName.push(v);
                    }
                }

                columnTitleTrs.push(resultName)
                return columnTitleTrs.concat(table);
            }
        }
    }
</script>

<style scoped>
    td {
        border: 1px solid #333;
    }

</style>
