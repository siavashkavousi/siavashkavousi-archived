<template>
  <div>
    <q-card class="shadow-1">
      <q-card-title class="text-secondary">
        <div class="row">
          <q-icon name="school" size="40px"></q-icon>
          <h3 class="pl-3">Education</h3>
        </div>
      </q-card-title>
      <q-card-main>
        <q-list>
          <q-item>
            <strong class="text-orange-9">Amirkabir University of Technology (AUT) - Tehran</strong>
            <div>Bachelor of Science – Enrolled September 2013</div>
            <div>Last year: 18.07/20</div>
            <div>Cumulative Grade Average: 15.5/20 (109/140 Units)</div>
            <!--<div>Major Grade Average: 15.62/20</div>-->
          </q-item>
          <q-item>
            <strong class="text-orange-9">Farabi High School – Gonbad-e-Qabus</strong>
            <div>Mathematics & Physics Diploma – Graduated July 2012</div>
            <div>GPA: 19.13/20</div>
          </q-item>
        </q-list>
      </q-card-main>

      <q-card-title>
        <h3 class="text-secondary">Research Interests</h3>
      </q-card-title>
      <q-card-main>
        <q-list>
          <q-item>Machine Learning</q-item>
          <q-item>Computer Vision</q-item>
          <q-item>Convolutional Neural Networks</q-item>
          <q-item>Deep Learning</q-item>
          <q-item>Statistics</q-item>
          <q-item>Linear Algebra</q-item>
          <q-item>Distributed Processing</q-item>
        </q-list>
      </q-card-main>

      <q-card-title class="text-secondary">
        <h3>Honors & Awards</h3>
      </q-card-title>
      <q-card-main>
        Ranked in 1% among more than 251,956 participators in Nation-wide University
        Entrance Exam among all Iranian Students of Math. & Physics (2013)
      </q-card-main>

      <q-card-title class="text-secondary">
        <h3>Professional Accomplishments</h3>
      </q-card-title>
      <q-card-main>
        <q-list>
          <q-item>
            <strong class="text-orange-9">Data Mining and Machine Learning</strong>
            <section>
              <em class="text-blue-7">Applications</em>
              <div class="pl-3">
                <div>Developing <strong>license plate recognizer</strong> for iranian car plates - In progress!</div>
                <div>Developing and testing <strong>DMC 2016</strong> problem with XGBoost, Keras, and Pandas</div>
                <div>Working with Apache Sparks in
                  <strong>Introduction to Apache Spark</strong>,
                  <strong>Big Data Analysis with Apache Spark</strong>
                  BerkeleyX online courses in edx.org
                </div>
                <div>Developing and working on Fanavard challenge problems</div>
                <div>Implementing HOG and Deformable parts model (Feature extraction)</div>
              </div>
              <em class="text-blue-7">Libraries and frameworks</em>
              <div class="pl-3">Tensorflow, Keras, Scipy, Scikit, Pandas, Apache Spark, XGBoost, Jupyter Notebook</div>
              <em class="text-blue-7">Challenges</em>
              <div class="pl-3">Fanavard 2016 (data mining national challenge)</div>
            </section>
          </q-item>
          <q-item>
            <strong class="text-orange-9">Web Development</strong>
            <section>
              <em class="text-blue-7">Projects</em>
              <!--<div>Customizing <strong>OpenEdx</strong> platform in order to use in our university</div>-->
              <div class="pl-3">Developing <strong>MOOC</strong> (massive open online courses) platform</div>
              <div class="pl-3">Developing a customized version of Apache Ofbiz named Redon based on the
                needs of a customer (Iran-NGK Spark Plug Supplier) in HISIS (Hoonam Intelligent Secure Integrated
                Systems) Company
              </div>
              <em class="text-blue-7">Libraries and frameworks</em>
              <div class="pl-3">Django, Backbone, Polymer, Laravel</div>
            </section>
          </q-item>
          <q-item>
            <strong class="text-orange-9">Android</strong>
            <section>
              <em class="text-blue-7">Applications</em>
              <q-list no-border dense>
                <q-item>
                  <div>DualCamera&nbsp;</div>
                  <div>(Android camera application in order to use both cameras and merge their photos together)</div>
                </q-item>
                <q-item>
                  <div>DubsmashFa&nbsp;</div>
                  <div>(Android application similar to Dubsmash but in Persian)</div>
                </q-item>
              </q-list>
              <em class="text-blue-7">Libraries and frameworks</em>
              <div class="pl-3">
                Retrofit, RxJAVA, RxAndroid, RxKotlin, Dagger 2, Picasso, Glide,
                Butterknife, Kotterknife, LeakCanary, OkHttp, Fabric
              </div>
              <em class="text-blue-7">Patterns and Architectures</em>
              <div class="pl-3">Reactive and functional programming, MVP(Model-View-Presenter)</div>
            </section>
          </q-item>
        </q-list>
      </q-card-main>


      <q-card-title class="text-secondary">
        <h3>Teaching Experiences & Presentations</h3>
      </q-card-title>
      <q-card-main>
        <q-list>
          <q-item>
            <strong class="text-orange-9">Presentation in 8th Amirkabir Linux Festival - July 2016 (<strong>Technical Commitee</strong>)</strong>
            <ul>
              <li>Introduction to Linux</li>
              <li>Intermediate and advanced bash programming</li>
            </ul>
          </q-item>
          <q-item>
            <strong class="text-orange-9">MongoDB introduction</strong>
            <div class="pl-3">Database Design Lab - November 2016</div>
          </q-item>

          <q-item>
            <strong class="text-orange-9">An Introduction to TensorFlow</strong>
            <div class="pl-3">8th Amirkabir Linux Festival - July 2016</div>
          </q-item>
          <q-item>
            <strong class="text-orange-9">Traffic sign recognition</strong>
            <div class="pl-3">Research methods and writing - June 2016</div>
          </q-item>
        </q-list>
      </q-card-main>

      <q-card-title class="text-secondary">
        <h3>Academic Course Projects</h3>
      </q-card-title>
      <q-card-main>
        <q-list>
          <q-item>
            <strong>Advanced programming</strong>
            <div>Developing Battleship, JDM (download manager), Hare and Tortoise game,
              JCalculator (calculator), Bubbles(Socket programming, Swing), Simple Text Editor
              (Swing), JOMUNG(Game using swing and network and DFS algorithm). These
              projects were done mainly using JAVA
            </div>
          </q-item>

          <q-item>
            <strong>Principles of programming</strong>
            <div>Developing Paint, Snake, Super Mario, Editor(English and Persian) and Calculator
              (with diagram drawer and using automaton) all in C++
            </div>
          </q-item>

          <q-item>
            <strong>Data structures and algorithms</strong>
            <div>Developing shared linked list for student information, Binary trees, B-Trees, AVL
              trees, Huffman compression using C++
            </div>
          </q-item>

          <q-item>
            <strong>Machine language programming</strong>
            <div>Finding password of an executable file and reverse it using TurboDebugger and
              HexEditor
              Developing GCD, Radical, Factorial, Fibonacci, Screen saver, Delay, Graphical Line,
              Bubble Sort using Assembly language
              Developing FAT16 file explorer using C#
            </div>
          </q-item>

          <q-item>
            <strong>Logic circuits</strong>
            <div>Developing division by 3 circuit using SystemVerilog
              RS232 protocol using SystemVerilog and Python
              Traffic light using proteus
            </div>
          </q-item>

          <q-item>
            <strong>Computer architectures</strong>
            <div>Developing Direct Mapped Cache using SystemVerilog, Developing ALU and
              Calculator using Proteus
            </div>
          </q-item>

          <q-item>
            <strong>Operating Systems</strong>
            <div>
              Adds process suspend and resume to <strong>XV6 MIT OS</strong>
              <a href="https://github.com/siavashkavousi/xv6-public"></a>
            </div>
          </q-item>

          <q-item>
            <strong>Convolutional Neural Networks for Visual Recognition</strong>
            <a href="https://github.com/siavashkavousi/CNN-course"></a>
            <div>Develops K-NN, Softmax, SVM and 2-Layer Neural Net classifier using Python
              Develops CNN classifier using Python
            </div>
          </q-item>

          <q-item>
            <strong>Principles of Database Design</strong>
            <a href="https://github.com/siavashkavousi/DB-course"></a>
            Implements an online music store database using MySQL
            <a href="https://github.com/siavashkavousi/MusicStoreDB"></a>
            Develops Messenger application (client/server, JavaFX for GUI, MongoDB for
            database)
            <a href="https://github.com/siavashkavousi/Messenger"></a>
          </q-item>

          <q-item>
            <strong>Microprocessors</strong>
            <a href="https://github.com/siavashkavousi/MP-course"></a>
            <div>Implements range finder with SRF02 sensor and AT-mega16 microcontroller using C</div>
          </q-item>

          <q-item>
            <strong>Advanced Mathematics</strong>
            <div>Implements facial recognition using SVD algorithm using Matlab</div>
          </q-item>

          <q-item>
            <strong>Internet Engineering (Web Development)</strong>
            <a href="https://github.com/siavashkavousi/IE-course"></a>
            <div>
              Develops AUT studio (game portal) using <strong>Laravel</strong> as backend and <strong>Polymer</strong>framework as frontend
            </div>
          </q-item>
        </q-list>
      </q-card-main>

      <q-card-title class="text-secondary">
        <h3>Online Education</h3>
      </q-card-title>
      <q-card-main>
        <q-list>
          <q-item>
            <strong>Machine Learning</strong>
            <a href="https://github.com/siavashkavousi/ML-course"></a>
          </q-item>
          Offered by Prof. Ng (Stanford University) – Grade=100%

          <q-item>
            <strong>Convolutional Neural Networks for Visual Recognition</strong>
            <a href="https://github.com/siavashkavousi/CNN-course"></a>
          </q-item>
          Offered by Prof. Fei Fei Li (Stanford University)

          <q-item><strong>Introduction to Apache Spark</strong></q-item>
          Offered by Prof. Anthony D. Joseph (UC Berkeley) - edx.org

          <q-item><strong>Big Data Analysis with Apache Spark</strong></q-item>
          Offered by Prof. Anthony D. Joseph (UC Berkeley) - edx.org

          <q-item><strong>Applied Data Science with Python - currently</strong></q-item>
          University of Michigan - Coursera
        </q-list>
      </q-card-main>

      <q-card-title class="text-secondary">
        <h3>Skills</h3>
      </q-card-title>
      <q-card-main>
        <q-list>
          <q-item>
            <strong>Programming</strong>
            <div>Experienced in Python, Matlab, JAVA, C/C++, Bash, Kotlin, Android, PHP, HTML, JavaScript, Groovy, CSS, Sass
            </div>
            <div>Familiar with C#, VHDL, Assembly, FTL, SystemVerilog</div>
          </q-item>

          <q-item>
            <strong>Operating Systems & Linux Technologies</strong>
            <div>Ubuntu, CentOS, Docker, Kubernetes, LXD, Windows</div>
          </q-item>

          <q-item>
            <strong>Typesetting</strong>
            <div><i class="glyphicon glyphicon-text-height"></i> LATEX, Microsoft Word</div>
          </q-item>

          <q-item>
            <strong>Language</strong>
            <ul>
              <li>Farsi (Persian) : Native</li>
              <li>English : Fluent</li>
            </ul>
          </q-item>
        </q-list>
      </q-card-main>
      <q-card-title class="text-secondary">
        <h3>References</h3>
      </q-card-title>
      <q-card-main>References are available upon request</q-card-main>
    </q-card>
  </div>
</template>

<script>
  import {
    QCard,
    QCardTitle,
    QCardMain,
    QIcon,
    QList,
    QItem
  } from 'quasar'

  export default {
    components: {
      QCard,
      QCardTitle,
      QCardMain,
      QIcon,
      QList,
      QItem
    }
  }
</script>

<style lang="stylus" scoped>
  .q-item
    flex-direction: column
    align-items flex-start
</style>
