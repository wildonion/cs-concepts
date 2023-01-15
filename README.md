## 📚 blogs and books:

* https://rust-unofficial.github.io/patterns/

* https://book.avr-rust.com/001-introduction.html
    
* https://nnethercote.github.io/perf-book/title-page.html

* https://rust-lang-nursery.github.io/rust-cookbook/intro.html
     
* https://smallcultfollowing.com/babysteps/
     
* https://lucumr.pocoo.org/
     
* https://www.lpalmieri.com/
     
* https://blog.yoshuawuyts.com/
     
* https://www.i-programmer.info/programming/theory.html
     
* https://www.i-programmer.info/babbages-bag/
     
* https://without.boats/blog/
    
## 📡 networking

#### 🛠️ tools:

* tokio

* impl riker actor for each socket connection

* libp2p pub/sub stack based on tokio tcp and udp with borsh and serde

* zmq pub/sub socket for async I/O event streaming like audio and video

* rpc capnp

* hyper

#### 🎭 actor concepts:
* mailbox to receive async messages from other actors and other part of the app  
* pub/sub channels for executing and scheduling async tasks 
* tokio worker green threadpool to run task in other threads
* rpc capnp based communication with outside world actors 
* tokio message queue channles like mpsc for sharing data between threads
* tokio event loop using select! to select an async I/O event task

#### 💡 concepts:

* distributed (replication) and decentralized concepts:
  * search, db and routing engines like elastic, cassandra and p2p kademlia: 
  * create best objective function to find the most rewarded (less cost actions) path in the network graph env (route planning) greedily using:
  * hybrid tech algorithms like NN, GA and neurofuzzy(ANFIS)
  * gradient optimization methods like stochastic gradient descent 
  * none gradient optimization methods like GA and FA
  * graph theory and heuristic search algorithms like DAG, dijkstras, floyd, bellman, DFS, BFS and A*
  * reinforcement learning algorithms like qlearning using mdp and bellman equation with off and on policy methods based on markov decision process and markov chain
  
  * other algorithms using greedy, dynamic programming, backtracking, divide and conquer, recursive and brute forcing methods
  * hashmap based algos like hash tables (DHT) to find closest peers inside a replication like cassandra db and p2p nodes    
  * rpc capnp for actor method based communication on two different machines like calling between smart contract actors
  * tokio tcp and udp and jobq channels for sharing Arc<Mutex<T>>: Send + Sync + 'static between actor threads in a same machine
  * actor tokio worker green threadpool and message queue for task and method broadcasting and scheduling to the pub/sub channels (tokio jobq, socket or rpc)
  * pub/sub and other zmq socket actors to broadcast from publishers to subscribers (m2m) using sockets
  * in libp2p peers can find each other using either mDNS (over LAN) or kademlia (over WAN)
 * in libp2p peers can communicate with each other based on pub/sub floodsub or gossipsub protocols on top of rpc capnp, tokio udp and tcp, websocket, webrtc, zmq like sockets (req/res, cli/srv or pub/sub) actors
 * proxy, firewall, vpns, packet sniffer and load balancer like pingora, HAproxy, v2ray and wireshark for all layers concepts:
   * v2ray and tor protocols
   * decompress encoded packet 
   * cpu task scheduling, 
   * weighted round robin dns, 
   * vector clock, 
   * event loop
   * iptables
   * zmq pub/sub
   * simd divide and conquer based vectorization
   
## 🏗️ system

  #### 💡 concepts:
  * compiler, vm using llvm and os
  * streaming of async I/O events compression and codec ram (buffer) algos like deflate, lz4, snappy, borsh, bson, serde and capnp
  * runtime
  * video and audio codec, compressor and streamer like ffmpeg
  * cryptography
  * bridge between blockchains
  * language binding like writing rust code on top of apis of the compiled (.so) code in c like rust bindings to libsodium
