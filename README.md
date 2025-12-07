# AMD_Robotics_Hackathon_2025_[Hardworking burger-cooking robot]

## Team Information

**Team:** *26, でんとつー,高岸司　米田久美子　オウカン*

**Summary:** *勤勉なハンバーガー調理ロボット（Hardworking burger-cooking robot）*

*プロジェクト紹介動画：*
*https://youtube.com/shorts/_USv2LYLnRU?si=Iba8shECn3K2kpP4*
*ハンバーガー屋で人と協力して働く勤勉な調理ロボットです。カメラを搭載した２台のアームを使って、ハンバーガーの組み立て作業を行います。*
*非常に仕事熱心なこのロボットはカメラで周囲の状況を監視し、周囲に働きぶりを監視する人がいるかどうかを判断します。周囲に監視を行う人がいる場合、バンズとレタスを１つずつ取り出し、ハンバーガーを組み立てます。*
*監視の目がないと、ハンバーガーの調理をやめ、タバコを吸い始めます。*

## Submission Details

### 1. Mission Description
*私たちは双腕のSO-101ロボットを用いてハンバーガーモデルの組み立てタスクの教示を収集し、ACTモデルを用いて模倣学習を行いました。*
*高速に料理を作ることが求められるファストフード店や、混雑時に作業負担が増えるシフトでの助けになります。ロボットが調理している間に、スタッフは他の業務に集中できます。*
### 2. Creativity
- *私たちの狙いはタスクの成功だけではありません。ロボットがハンバーガーを組み立てる姿に加えて、「サボる」仕草をエンターテイメント要素として活用することを考えています。*
- *テーマパークなどエンターテイメント業界ではロボットが大活躍しています。このプロジェクトでは客の前でロボットがハンバーガーを作ったり、サボったりするパフォーマンスを行い、来店客に楽しんでもらうためのロボットショーとして、「働きすぎない」姿を見せて笑いを誘うことができます。このプロジェクトを通してロボットに『感情』や『意図』を持たせることを挑戦しました。*

### 3. Technical implementations

*教示の動画：*
*https://youtube.com/shorts/uIRNWiMA8Sk?si=K4jXW-STPEhbf3mW*
*【トレーニング】*
*教示の多峰性を回避し安定した動作を獲得するため、事前に決めた軌跡を描くようにデータを収集しました。*
*最終日に照明環境やカメラの位置ずれにより２日目に学習したモデルが正確に動作、追加で教示を収集して追加学習することで高い再現性を*実現しました。*
*【アルゴリズム】*
*ロボットアームが人を探す行動はleader-followerで記録したデータから再生するようにしています。アームについているカメラを用いて人間がいるかどうかをopenCVで検出し、次の行動を決めます。*
*【ハードウェア】*
*・fusion360を用いてハンバーガー供給用ロータリーテーブルやその他小物を設計しました。*
*・設計した部品は会場にBambuA1miniを持参し、作成しました。*
*・ロータリーテーブルの回転機構にはRoboStrideモーターを使用しました。*
*タスクの実行動画：*
*https://youtube.com/shorts/0LJgFBQEfmY?si=bgUAgur_pWV35PwN*

### 4. Ease of use
*burger/main.pyを実行してすることでDEMOを再生できます。*

## Additional Links
*プロジェクト紹介動画：*
*https://youtube.com/shorts/_USv2LYLnRU?si=Iba8shECn3K2kpP4*

 *教示の動画：*
*https://youtube.com/shorts/uIRNWiMA8Sk?si=K4jXW-STPEhbf3mW*

*タスクの実行動画：*
*https://youtube.com/shorts/0LJgFBQEfmY?si=bgUAgur_pWV35PwN*

*学習データセット：*
*Mozgi512/burger_merged2*
*Mozgi512/burger4(追加学習)*
*学習済みモデル：*
*Mozgi512/act_burger_final_8000*


