FROM noasking/centos74-opencv340-java8
VOLUME /tmp
ARG JAR_FILE
ADD ${JAR_FILE} app.jar
RUN cp /opencv/release/share/OpenCV/java/libopencv_java340.so /usr/local/lib/
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app/app.jar"]