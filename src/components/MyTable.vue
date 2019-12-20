<template>
    <div >
        <table>
            <thead></thead>
            <tbody>
                <tr v-for="item of tableList">
                    <td v-for="i of item">
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
        data(){
            return {
                tableList:[]
            }
        },
        created() {
            let dataConfig = {"rows":[{"columnName":"area","alias":"区","filterType":"eq","values":[],"id":"zsuuvzmp3joanbjeepvmj4xe6bggp57t"},{"columnName":"year","alias":"年","filterType":"eq","values":[],"id":"lnfovnxah3yqvnkn6s4grhu8fpa1rzio"},{"columnName":"age_group","alias":"分组类型","filterType":"eq","values":[],"id":"ldznt1stolnkwbtmr13l1hns6fa9mkzg"}],"columns":[{"columnName":"audit_state","alias":"审核状态","filterType":"eq","values":[],"id":"ptdnrxnj2bwbrkjsmhxu2d3lc4437dzq"}],"filters":[],"values":[{"column":"male_num","alias":"男性人口数","aggType":"max"}]}
            let dataList = {"columnList":[{"index":0,"aggType":null,"name":"audit_state","alias":"审核状态"},{"index":1,"aggType":null,"name":"area","alias":"区"},{"index":2,"aggType":null,"name":"year","alias":"年"},{"index":3,"aggType":null,"name":"age_group","alias":"分组类型"},{"index":4,"aggType":"max","name":"male_num","alias":"男性人口数"}],"data":[["二审通过","海珠区","2017","0-","3583"],["二审通过","海珠区","2017","1-","4374"],["二审通过","海珠区","2017","10-","12005"],["二审通过","海珠区","2017","15-","13684"],["二审通过","海珠区","2017","2-","3601"],["二审通过","海珠区","2017","20-","17763"],["二审通过","海珠区","2017","25-","24709"],["二审通过","海珠区","2017","3-","3445"],["二审通过","海珠区","2017","30-","28049"],["二审通过","海珠区","2017","35-","23709"],["二审通过","海珠区","2017","4-","3186"],["二审通过","海珠区","2017","40-","21619"],["二审通过","海珠区","2017","45-","27491"],["二审通过","海珠区","2017","5-","3571"],["二审通过","海珠区","2017","50-","31039"],["二审通过","海珠区","2017","55-","36632"],["二审通过","海珠区","2017","6-","2891"],["二审通过","海珠区","2017","60-","35177"],["二审通过","海珠区","2017","65-","22168"],["二审通过","海珠区","2017","7-","2742"],["二审通过","海珠区","2017","70-","13201"],["二审通过","海珠区","2017","75-","9233"],["二审通过","海珠区","2017","8-","2380"],["二审通过","海珠区","2017","80-","7831"],["二审通过","海珠区","2017","85及以上","5878"],["二审通过","海珠区","2017","9-","2673"],["二审通过","海珠区","2017","合计","362634"],["二审通过","荔湾区","2017","0-","5298"],["二审通过","荔湾区","2017","1-","6811"],["二审通过","荔湾区","2017","10-","21687"],["二审通过","荔湾区","2017","15-","23418"],["二审通过","荔湾区","2017","2-","5593"],["二审通过","荔湾区","2017","20-","29272"],["二审通过","荔湾区","2017","25-","43290"],["二审通过","荔湾区","2017","3-","5293"],["二审通过","荔湾区","2017","30-","43008"],["二审通过","荔湾区","2017","35-","40950"],["二审通过","荔湾区","2017","4-","5086"],["二审通过","荔湾区","2017","40-","38773"],["二审通过","荔湾区","2017","45-","48990"],["二审通过","荔湾区","2017","5-","5944"],["二审通过","荔湾区","2017","50-","49338"],["二审通过","荔湾区","2017","55-","49918"],["二审通过","荔湾区","2017","6-","5273"],["二审通过","荔湾区","2017","60-","48045"],["二审通过","荔湾区","2017","65-","32205"],["二审通过","荔湾区","2017","7-","4980"],["二审通过","荔湾区","2017","70-","18307"],["二审通过","荔湾区","2017","75-","14869"],["二审通过","荔湾区","2017","8-","4513"],["二审通过","荔湾区","2017","80-","13666"],["二审通过","荔湾区","2017","85及以上","10357"],["二审通过","荔湾区","2017","9-","5067"],["二审通过","荔湾区","2017","合计","579951"],["未提交审核","荔湾区","2017","0-","3583"],["未提交审核","荔湾区","2017","1-","4374"],["未提交审核","荔湾区","2017","10-","12005"],["未提交审核","荔湾区","2017","15-","13684"],["未提交审核","荔湾区","2017","2-","3601"],["未提交审核","荔湾区","2017","20-","17763"],["未提交审核","荔湾区","2017","25-","24709"],["未提交审核","荔湾区","2017","3-","3445"],["未提交审核","荔湾区","2017","30-","28049"],["未提交审核","荔湾区","2017","35-","23709"],["未提交审核","荔湾区","2017","4-","3186"],["未提交审核","荔湾区","2017","40-","21619"],["未提交审核","荔湾区","2017","45-","27491"],["未提交审核","荔湾区","2017","5-","3571"],["未提交审核","荔湾区","2017","50-","31039"],["未提交审核","荔湾区","2017","55-","36632"],["未提交审核","荔湾区","2017","6-","2891"],["未提交审核","荔湾区","2017","60-","35177"],["未提交审核","荔湾区","2017","65-","22168"],["未提交审核","荔湾区","2017","7-","2742"],["未提交审核","荔湾区","2017","70-","13201"],["未提交审核","荔湾区","2017","75-",null],["未提交审核","荔湾区","2017","8-","2380"],["未提交审核","荔湾区","2017","80-","7831"],["未提交审核","荔湾区","2017","85及以上","5878"],["未提交审核","荔湾区","2017","9-","2673"],["未提交审核","荔湾区","2017","合计","362634"]]}
            let rows = dataConfig.rows.map(op => {
                return op.columnName
            })
            let columns = dataConfig.columns.map(op => {
                return op.columnName
            })
            let values = dataConfig.values.map(op => {
                return op.column
            })

            this.tableList = this.convertToTable(dataList, rows, columns, values);
            for (let tr of this.tableList) {
                //console.log(tr);
            }
        },
        methods:{
            convertToTable(dataList, rows, columns, values) {
                let columnIndexMap = new Map();
                for (let c of dataList.columnList) {
                    columnIndexMap.set(c.name, c);
                }
                let data = dataList.data;

                let tableMap = new Map();
                let rowTitleMap = new Map();
                let columnTitleMap = new Map();

                function check(d,arrs,titleMap) {
                    let key = ''
                    let i =0;
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

                    let trKey = check(d,rows,rowTitleMap);
                    let tdKey = check(d,columns,columnTitleMap);

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

                function getTitles(trs, titleArr,map,pre,index) {
                    if (pre === null || pre === undefined) {
                        pre = '';
                    }
                    if (index === null || index === undefined) {
                        index = 0;
                    }
                    let tr = trs[index];
                    for (let [k,v] of map.entries()) {
                        if (v === null || v === undefined || v.size === 0) {
                            titleArr.push(pre + k);
                            tr.push({name:k, c: 0})
                        }else{
                            tr.push({name:k, c: v.size})
                            getTitles(trs,titleArr, v, pre + k + '_', index + 1);
                        }
                    }
                }

                let rowTitleArr = [];
                let columnTitleArr =[]

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

                getTitles(rowTitleTrs,rowTitleArr, rowTitleMap);
                getTitles(columnTitleTrs,columnTitleArr, columnTitleMap);

                function patchEmpty(arr) {
                    if (arr === null || arr === undefined || arr.length === 0) {
                        return;
                    }
                    let needPatchArr = [];
                    for (let a of arr) {
                        if (a.c && a.c > 1) {
                            needPatchArr.push(a);
                        }
                    }
                    if (needPatchArr.length === 0) {
                        return;
                    }
                    for (let n of needPatchArr) {
                        let find = arr.filter((i) => i.name === n.name)[0];
                        if (find) {
                            let index = arr.indexOf(find) + 1;
                            let c = n.c - 1;
                            for (let j = 0; j < c; j++) {
                                arr.splice(index + j, 0, {});
                            }
                        }
                    }
                }

                /*for (let tr of rowTitleTrs) {
                    patchEmpty(tr)
                }
                for (let tr of columnTitleTrs) {
                    patchEmpty(tr);
                }*/


                let convertedRowTitleTrs = new Map();

                for (let i = 0; i < rowTitleArr.length; i++) {
                    let arr = [];
                    for (let a of rowTitleTrs) {
                        arr.push(a[i]);
                    }
                    convertedRowTitleTrs.set(rowTitleArr[i], arr);
                }

                let table = [];
                for (let [trKey,trMap] of tableMap.entries()) {
                    let tr = convertedRowTitleTrs.get(trKey) || [];
                    for (let columnKey of columnTitleArr) {
                        let td = trMap.get(columnKey);
                        if (td === null || td === undefined) {
                            for (let j = 0; j < values.length; j++) {
                                tr.push(0);
                            }
                        }else{
                            for (let v of values) {
                                tr.push(td.get(v));
                            }
                        }
                    }
                    table.push(tr)
                }

                let resultName = [];

                for (let a of rows) {
                    resultName.push(a);
                }
                for (let a of columnTitleArr) {
                    for (let j = 0; j < values.length; j++) {
                        resultName.push(a);
                    }
                }
                columnTitleTrs.push(resultName)
                return columnTitleTrs.concat(table);
            }
        }
    }
</script>

<style scoped>
    td{
        border: 1px solid #333;
    }

</style>
