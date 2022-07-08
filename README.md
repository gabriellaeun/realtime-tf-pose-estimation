Hey! This is a clone of the tf-pose-estimation by Ildoo Kim modified to work with Tensorflow 2.0+!
Link to original repo: https://www.github.com/ildoonet/tf-openpose
Link to another repo: https://github.com/gsethi2409/tf-pose-estimation


[manual 정리]
https://prabhjotkaurgosal.com/human-pose-estimation-using-openpose/
링크 참고

https://su0-0su.tistory.com/97
에러 수정은 이거 참고함

+opencv 에러 생기면 이거 보기
https://yongku.tistory.com/entry/PYTHON-No-module-named-cv2-%EB%AC%B8%EC%A0%9C-%ED%95%B4%EA%B2%B0%ED%95%98%EA%B8%B0

+wheel 다운로드는
pip install opencv-contrib-python 
이거 복붙 ( https://stackoverflow.com/questions/51203537/opencv-python-3-4-2contrib-cp37-cp37m-win-amd64-whl-is-not-a-supported-wheel-on )


마지막까지 속 썩인 GlorotUniform() 이거는 glorot_uniform()으로 바꿔줬더니 바로 됨…
https://www.tensorflow.org/api_docs/python/tf/compat/v1/keras/initializers/glorot_uniform
그리고 initializers 관련해서
initializer = tf.compat.v1.keras.initializers.TruncatedNormal()
이거로 바꿔줌
참고
https://stackoverflow.com/questions/65021316/attributeerror-module-tensorflow-api-v1-initializers-has-no-attribute-trunc

