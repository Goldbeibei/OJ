<template>
  <panel>
    <div slot="title">{{$t('m.Frequently_Asked_Questions')}}</div>
    <div class="content markdown-body">
      <ul>
        <li>{{$t('m.Where_is_the_input_and_the_output')}} 
          <p>{{$t('m.Where_is_the_input_and_the_output_answer_part_1')}} <code>stdin</code> ('{{$t('m.Standard_Input')}}') {{$t('m.Where_is_the_input_and_the_output_answer_part_3')}} <code>stdout</code>
            ('{{$t('m.Standard_Output')}}') {{$t('m.Where_is_the_input_and_the_output_answer_part_5')}} <code>scanf</code> {{$t('m.Where_is_the_input_and_the_output_answer_part_6')}} <code>cin</code>
            {{$t('m.Where_is_the_input_and_the_output_answer_part_7')}} <code>printf</code> {{$t('m.Where_is_the_input_and_the_output_answer_part_8')}} <code>cout</code> {{$t('m.Where_is_the_input_and_the_output_answer_part_9')}} <code>{{$t('m.Runtime_Error')}}</code>.
          </p>
        </li>
        <li>「穩點」是什麼？
          <p>「穩健 OnlineJudge」的穩點系統。
		        您可以通過簽到、做題來獲取穩點，到達一定穩點可以升級，並獲得等級稱號。
          </p>
          <p>穩點計算說明:
            <p>1、簽到每次獲得 <code>1</code> 穩點。在連續簽到的第 <code>3、7、15、30、60、90、120、240、365</code> 天可以分別額外獲得 <code>1、2、4、7、12、20、33、54、88</code> 穩點（沒錯，就是斐波那契數列）；</p>
            <p>2、每道題目，<strong>第一次 AC </strong>時根據難度（Low、Mid、High），可分別獲得 <code>3、8、15</code> 穩點。 </p>
          </p>
          <p>
            等級稱號如下：
            <p>0 - 99 穩點: <Tag color="#636e72" style="margin-right:-15px;">小白兔</Tag></p>
            <p>100 - 199 穩點: <Tag color="primary" style="margin-right:-15px;">菜鳥</Tag></p>
            <p>200 - 499 穩點: <Tag color="#6c5ce7" style="margin-right:-15px;">鍵盤蝦</Tag></p>
            <p>500 - 999 穩點: <Tag color="#1dd1a1" style="margin-right:-15px;">馬農</Tag></p>
            <p>1000 - 4999 穩點: <Tag color="#ff9f43" style="margin-right:-15px;">牛人</Tag></p>
            <p>5000 - 9999 穩點: <Tag color="#ee5253" style="margin-right:-15px;">程序猿</Tag></p>
            <p>10000 - ∞ 穩點: <Tag color="#222f3e" style="margin-right:-15px;">攻城獅</Tag></p>
            <p>分別是0 - 6級（程序猿都是從 0 開始的嘛），每個等級都有自己的稱號</p>
          </p>
        </li>
        <li>{{$t('m.What_is_the_meaning_of_submission_execution_time')}} 
        <p>{{$t('m.What_is_the_meaning_of_submission_execution_time_answer')}} 
        </p>
        </li>
        <li>{{$t('m.How_Can_I_use_CPP_Int64')}} 
          <p>{{$t('m.How_Can_I_use_CPP_Int64_answer_part_1')}}<code>long long</code> {{$t('m.How_Can_I_use_CPP_Int64_answer_part_2')}} <code>cin/cout</code> {{$t('m.or')}} <code>%lld</code>, {{$t('m.using')}}<code> __int64</code> {{$t('m.How_Can_I_use_CPP_Int64_answer_part_3')}} <code>{{$t('m.Compile_Error')}}</code>.</p>
        </li>
        <li>{{$t('m.Java_specifications')}}
          <p>{{$t('m.Java_specifications_answer_part_1')}} <code>Main</code> {{$t('m.Java_specifications_answer_part_2')}} <code>Main</code> {{$t('m.Java_specifications_answer_part_3')}}</p>
        </li>
        <li>{{$t('m.About_presentation_error')}}
          <p>{{$t('m.About_presentation_error_answer_part_1')}} <b>{{$t('m.last')}}</b> {{$t('m.About_presentation_error_answer_part_2')}} <code> {{$t('m.Wrong_Answer')}}</code>.</p>
        </li>
        <li>{{$t('m.How_to_report_bugs')}}
          <p>{{$t('m.How_to_report_bugs_answer_part_1')}} <a href="https://github.com/Harry-zklcdc/OnlineJudge">Github</a>
            {{$t('m.How_to_report_bugs_answer_part_2')}}
          </p>
        </li>
      </ul>
    </div>
  </panel>
</template>

<script>
</script>

<style lang="less" scoped>
  .content {
    font-size: 16px;
    margin: 0 50px 40px 50px;
    > ul {
      list-style: disc;
      li {
        font-size: 16px;
        margin-top: 20px;
        &:first-child {
          margin-top: 0;
        }
        p {
          font-size: 14px;
          margin-top: 5px;
        }
      }
    }
  }
</style>