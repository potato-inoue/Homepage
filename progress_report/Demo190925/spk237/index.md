# Speaker adaptation for single speaker tts model

model: ljspeech.transformer.v1
text: ASR output
speech: speech of target speaker

## 237(F)

| rev | 1 | 2 |  
| --- | --- | --- |  
| lr | 1e0 | 1e-1 |  
| epoch | 100 | 100 |  
| all_loss      | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/results/all_loss.png" width="320px">           | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1e-1.rev2/results/all_loss.png" width="320px">            |  
| loss          | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/results/loss.png" width="320px">               | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1e-1.rev2/results/loss.png" width="320px">                |  
| l1_loss       | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/results/l1_loss.png" width="320px">            | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1e-1.rev2/results/l1_loss.png" width="320px">             |  
| l2_loss       | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/results/l2_loss.png" width="320px">            | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1e-1.rev2/results/l2_loss.png" width="320px">             |  
| bce_loss      | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/results/bce_loss.png" width="320px">           | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1e-1.rev2/results/bce_loss.png" width="320px">            |  
| encoder_alpha | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/results/encoder_alpha.png" width="320px">      | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1e-1.rev2/results/encoder_alpha.png" width="320px">       |  
| decoder_alpha | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/results/decoder_alpha.png" width="320px">      | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1e-1.rev2/results/decoder_alpha.png" width="320px">       |  
| attn_loss     | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/results/enc_dec_attn_loss.png" width="320px">  | <img src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1e-1.rev2/results/enc_dec_attn_loss.png" width="320px">   |  

### target for pre-train  
<audio src="../ljspeech_asrtts_offline/ljspeech.ground_truth/eval/wav/LJ050-0029.wav" controls></audio>  

### 237_134500_000036_000000.wav  

    Ground truth: Marie clasped her hands and started up from her seat. 
    Recog output: MARIE CLASPED HER HANDS AND STARTED UP FROM HER SEAT. 

| type | wav |  
| --- | --- |  
| target for fine-tuning            | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237.ground_truth/eval/wav/237_134500_000036_000000.wav" controls></audio> |  
| 0th decode                        | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/eval_0th/wav/237_134500_000036_000000.wav" controls></audio> | 
| avg.best  (lr:1e0, 100 epoch)     | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/eval_avg.best/wav/237_134500_000036_000000.wav" controls></audio> |  
| avg.best  (lr:1e-1, 100 epoch)    | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1e-1.rev2/eval_avg.best/wav/237_134500_000036_000000.wav" controls></audio> |  

### 237_134500_000036_000001.wav  

    Ground truth: She had grown very pale and her eyes were shining with excitement and distress. "But, Emil, if I understand, then all our good times are over, we can never do nice things together any more. 
    Recog output: SHE HAD GROWN VERY PALE AND HER EYES WERE SHINING WITH EXCITEMENT AND DISTRESS BUT EMIL IF I UNDERSTAND AND ALL OUR GOOD TIMES ARE OVER WE CAN NEVER DO NICE THINGS TOGETHER ANY MORE. 

| type | wav |  
| --- | --- |  
| target for fine-tuning            | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237.ground_truth/eval/wav/237_134500_000036_000001.wav" controls></audio> |  
| 0th decode                        | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/eval_0th/wav/237_134500_000036_000001.wav" controls></audio> |  
| avg.best  (lr:1e0, 100 epoch)     | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/eval_avg.best/wav/237_134500_000036_000001.wav" controls></audio> |  
| avg.best  (lr:1e-1, 100 epoch)    | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1e-1.rev2/eval_avg.best/wav/237_134500_000036_000001.wav" controls></audio> |  

### 237_134500_000036_000002.wav  

    Ground truth: We shall have to behave like mr Linstrum. 
    Recog output: WE SHALL HAVE TO BEHAVE LIKE MISTER LINDSTROM. 

| type | wav |  
| --- | --- |  
| target for fine-tuning            | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237.ground_truth/eval/wav/237_134500_000036_000002.wav" controls></audio> |  
| 0th decode                        | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/eval_0th/wav/237_134500_000036_000002.wav" controls></audio> |  
| avg.best  (lr:1e0, 100 epoch)     | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/eval_avg.best/wav/237_134500_000036_000002.wav" controls></audio> |  
| avg.best  (lr:1e-1, 100 epoch)    | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1e-1.rev2/eval_avg.best/wav/237_134500_000036_000002.wav" controls></audio> |  

### 237_134500_000036_000003.wav  

    Ground truth: And, anyhow, there's nothing to understand!" She struck the ground with her little foot fiercely. 
    Recog output: AND ANYHOW THERE'S NOTHING TO UNDERSTAND SHE STRUCK THE GROUND WITH HER LITTLE FOOT FIERCELY. 

| type | wav |  
| --- | --- |  
| target for fine-tuning            | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237.ground_truth/eval/wav/237_134500_000036_000003.wav" controls></audio> |  
| 0th decode                        | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/eval_0th/wav/237_134500_000036_000003.wav" controls></audio> |  
| avg.best  (lr:1e0, 100 epoch)     | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/eval_avg.best/wav/237_134500_000036_000003.wav" controls></audio> |  
| avg.best  (lr:1e-1, 100 epoch)    | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1e-1.rev2/eval_avg.best/wav/237_134500_000036_000003.wav" controls></audio> |  

### 237_134500_000036_000004.wav  

    Ground truth: "That won't last. 
    Recog output: THAT WON'T LAST. 

| type | wav |  
| --- | --- |  
| target for fine-tuning            | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237.ground_truth/eval/wav/237_134500_000036_000004.wav" controls></audio> |  
| 0th decode                        | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/eval_0th/wav/237_134500_000036_000004.wav" controls></audio> |  
| avg.best  (lr:1e0, 100 epoch)     | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1.rev1/eval_avg.best/wav/237_134500_000036_000004.wav" controls></audio> |  
| avg.best  (lr:1e-1, 100 epoch)    | <audio src="../ljspeech_asrtts_offline/test_clean_22050_237_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk237_lr1e-1.rev2/eval_avg.best/wav/237_134500_000036_000004.wav" controls></audio> |  
