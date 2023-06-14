# Comparing `tmp/rlviser_py-0.2.0.tar.gz` & `tmp/rlviser_py-0.2.2.tar.gz`

## Comparing `rlviser_py-0.2.0.tar` & `rlviser_py-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 rlviser_py-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123     2774 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/.gitignore
--rw-r--r--   0     1001      123     1070 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/LICENSE
--rw-r--r--   0     1001      123      490 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/README.md
--rw-r--r--   0     1001      123      390 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123      255 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/rlviser_py.pyi
--rw-r--r--   0     1001      123       74 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/rustfmt.toml
--rw-r--r--   0     1001      123    32938 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/src/bytes.rs
--rw-r--r--   0     1001      123      995 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/src/gym.rs
--rw-r--r--   0     1001      123     4219 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123     1351 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/src/socket.rs
--rw-r--r--   0     1001      123     7635 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 rlviser_py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 rlviser_py-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      123     2774 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/.gitignore
+-rw-r--r--   0     1001      123     1070 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/LICENSE
+-rw-r--r--   0     1001      123      490 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/README.md
+-rw-r--r--   0     1001      123      390 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/pyproject.toml
+-rw-r--r--   0     1001      123      255 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/rlviser_py.pyi
+-rw-r--r--   0     1001      123       74 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/rustfmt.toml
+-rw-r--r--   0     1001      123    32938 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/src/bytes.rs
+-rw-r--r--   0     1001      123      995 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/src/gym.rs
+-rw-r--r--   0     1001      123     4269 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/src/lib.rs
+-rw-r--r--   0     1001      123     1443 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/src/socket.rs
+-rw-r--r--   0     1001      123     7635 2023-06-14 15:34:41.000000 rlviser_py-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 rlviser_py-0.2.2/PKG-INFO
```

### Comparing `rlviser_py-0.2.0/Cargo.toml` & `rlviser_py-0.2.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rlviser-py"
-version = "0.2.0"
+version = "0.2.2"
 edition = "2021"
 description = "Python implementation that manages a UDP connection to RLViser"
 license = "MIT"
 repository = "https://github.com/VirxEC/rlviser-py"
 readme = "README.md"
 keywords = ["rlviser", "rocket-league", "udp", "python", "rlbot"]
 publish = false
```

### Comparing `rlviser_py-0.2.0/.github/workflows/CI.yml` & `rlviser_py-0.2.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.2.0/.gitignore` & `rlviser_py-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.2.0/LICENSE` & `rlviser_py-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.2.0/src/bytes.rs` & `rlviser_py-0.2.2/src/bytes.rs`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.2.0/src/gym.rs` & `rlviser_py-0.2.2/src/gym.rs`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.2.0/src/lib.rs` & `rlviser_py-0.2.2/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -68,36 +68,31 @@
         suspension_rest_length: 37.055,
         connection_point_offset: Vec3A::new(-33.75, 29.5, 20.755),
     },
     dodge_deadzone: 0.5,
 };
 
 #[inline]
-fn ball_to_quat(array: [f32; 4]) -> Quat {
-    Quat::from_xyzw(array[1], array[2], array[3], array[0])
-}
-
-#[inline]
-fn car_to_mat3a(array: [f32; 4]) -> Mat3A {
-    Mat3A::from_quat(Quat::from_xyzw(-array[1], array[2], array[3], array[0]))
+fn array_to_quat(array: [f32; 4]) -> Quat {
+    Quat::from_xyzw(-array[1], -array[2], array[3], array[0])
 }
 
 /// Reads the RLGym state and sends it to RLViser to render
 #[pyfunction]
 fn render_rlgym(gym_state: GymState) {
     // construct the game state
     let game_state = GameState {
         tick_count: TICK_COUNT.fetch_add(1, Ordering::SeqCst),
         tick_rate: TICK_RATE,
         ball: BallState {
             pos: gym_state.ball.position.into(),
             vel: gym_state.ball.linear_velocity.into(),
             ang_vel: gym_state.ball.angular_velocity.into(),
         },
-        ball_rot: ball_to_quat(gym_state.ball.quaternion),
+        ball_rot: array_to_quat(gym_state.ball.quaternion),
         pads: BOOST_PAD_LOCATIONS
             .read()
             .unwrap()
             .into_iter()
             .zip(gym_state.boost_pads.into_iter())
             .map(|(position, is_active)| BoostPad {
                 position,
@@ -115,16 +110,19 @@
             .map(|(id, player)| CarInfo {
                 id: id as u32 + 1,
                 team: if player.team_num < 0.5 { Team::Blue } else { Team::Orange },
                 state: CarState {
                     pos: player.car_data.position.into(),
                     vel: player.car_data.linear_velocity.into(),
                     ang_vel: player.car_data.angular_velocity.into(),
-                    rot_mat: car_to_mat3a(player.car_data.quaternion),
+                    rot_mat: Mat3A::from_quat(array_to_quat(player.car_data.quaternion)),
                     is_on_ground: player.on_ground != 0,
+                    is_demoed: player.is_demoed != 0,
+                    has_flipped: player.has_flip == 0,
+                    has_jumped: player.has_jump == 0,
                     ..Default::default()
                 },
                 config: OCTANE,
             })
             .collect(),
     };
```

### Comparing `rlviser_py-0.2.0/src/socket.rs` & `rlviser_py-0.2.2/src/socket.rs`

 * *Files 18% similar despite different names*

```diff
@@ -15,20 +15,22 @@
 
 const RLVISER_PATH: &str = if cfg!(windows) { "./rlviser.exe" } else { "./rlviser" };
 
 static SOCKET: RwLock<Lazy<(UdpSocket, SocketAddr)>> = RwLock::new(Lazy::new(|| init().unwrap()));
 
 pub fn init() -> io::Result<(UdpSocket, SocketAddr)> {
     // launch RLViser
-    Command::new(RLVISER_PATH).spawn()?;
+    if let Err(e) = Command::new(RLVISER_PATH).spawn() {
+        println!("Failed to launch RLViser ({RLVISER_PATH}): {e}");
+    }
 
     // Connect to RLViser
     let socket = UdpSocket::bind("0.0.0.0:34254")?;
 
-    println!("Waiting for RLViser to connect...");
+    println!("Waiting for connection to socket...");
     let mut buf = [0; 1];
     let (_, src) = socket.recv_from(&mut buf)?;
 
     if buf[0] == 1 {
         println!("Connection established to {src}");
     }
```

### Comparing `rlviser_py-0.2.0/Cargo.lock` & `rlviser_py-0.2.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rlviser-py"
-version = "0.2.0"
+version = "0.2.2"
 dependencies = [
  "glam",
  "once_cell",
  "pyo3",
 ]
 
 [[package]]
```

### Comparing `rlviser_py-0.2.0/PKG-INFO` & `rlviser_py-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlviser-py
-Version: 0.2.0
+Version: 0.2.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python implementation that manages a UDP connection to RLViser
 Keywords: rlviser,rocket-league,udp,python,rlbot
 License: MIT
```

