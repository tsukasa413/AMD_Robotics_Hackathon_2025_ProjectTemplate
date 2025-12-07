**### Make a fork or copy of this repo and fill in your team submission details! ###**

# AMD_Robotics_Hackathon_2025_[Project Name]

## Team Information

**Team:** *26, でんとつー,高岸司　米田久美子　オウカン*

**Summary:** *勤勉なハンバーガー調理ロボット
（Hardworking burger-cooking robot）*

*<video src="./assets/story.mov" width="500" controls></video>*
ハンバーガー屋で人と協力して働く勤勉な調理ロボットです。カメラを搭載した２台のアームを使って、ハンバーガーの組み立て作業を行います。
非常に仕事熱心なこのロボットはカメラで周囲の状況を監視し、周囲に働きぶりを監視する人がいるかどうかを判断します。周囲に監視を行う人がいる場合、バンズとレタスを１つずつ取り出し、ハンバーガーを組み立てます。
監視の目がないと、ハンバーガーの調理をやめ、タバコを吸い始めます。

## Submission Details

### 1. Mission Description
*私たちは双腕のSO-101ロボットを用いてハンバーガーモデルの組み立てタスクの教示を収集し、ACTモデルを用いて模倣学習を行いました。
高速に料理を作ることが求められるファストフード店や、混雑時に作業負担が増えるシフトでの助けになります。ロボットが調理している間に、スタッフは他の業務に集中できます。*
### 2. Creativity
- *私たちの狙いはタスクの成功だけではありません。ロボットがハンバーガーを組み立てる姿に加えて、「サボる」仕草をエンターテイメント要素として活用することを考えています。*
- *Innovation in design, methodology, or application*


### 3. Technical implementations
- *Teleoperation / Dataset capture*
    - *<Image/video of teleoperation or dataset capture>*

    教示の多峰性を回避し安定した動作を獲得するため、事前に決めた軌跡を描くようにデータを収集しました。
    最終日に照明環境やカメラの位置ずれにより２日目に学習したモデルが正確に動作せず、追加で教示を収集して追加学習することで高い再現性を実現しました。
    人を探す行動はデータの再生することで
    【ハードウェア】
    ・fusion360を用いてハンバーガー供給用ロータリーテーブルやその他小物を設計しました。
    ・設計した部品は会場にBambuA1miniを持参し、作成しました。
    ・ロータリーテーブルの回転機構にはRoboStrideモーターを使用しました。
- *Training*
- *Inference*
    - *<Image/video of inference eval>*

### 4. Ease of use
左腕にあるカメラで人がいるか
- *Flexibility and adaptability of the solution*
- *Types of commands or interfaces needed to control the robot*

## Additional Links
*学習データセット：*
*Mozgi512/burger_merged2*
*Mozgi512/burger4(追加学習)*
*学習済みモデル：*
*Mozgi512/act_burger_final_8000*


