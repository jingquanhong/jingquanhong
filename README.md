<div align="center">

# Hi, I'm Jingquan Hong 👋

**人形机器人 · 视觉语言导航 · 世界模型**

Robotics Engineering (B.Eng., CQU) · Control Science and Engineering (M.Eng., NUDT)

[![Bruce & H-JEPA](https://img.shields.io/badge/Featured-Bruce%20%26%20H--JEPA%20in%20World%20Model-crimson?style=for-the-badge)](https://github.com/jingquanhong/bruce-H-JEPA-in-World-Model)

</div>

---

## 🔥 Bruce & H-JEPA in World Model

> 面向人形机器人的世界模型：从 Genesis 仿真越障数据采集，到实机 IMU 运动估计。
> **零训练、纯内推演**——不依赖强化学习试错，而是把越障动作解算成可解析复现的轨迹，并对每一步做物理复核。

[仓库地址](https://github.com/jingquanhong/bruce-H-JEPA-in-World-Model) · [数据集与采集管线](https://github.com/jingquanhong/bruce-H-JEPA-in-World-Model#采集管线) · [已知限制](https://github.com/jingquanhong/bruce-H-JEPA-in-World-Model#已知限制)

### 实机：IMU 前进 / 后退

<div align="center">
  <table>
    <tr>
      <td align="center" width="50%">
        <video width="380" controls preload="metadata"
          poster="https://raw.githubusercontent.com/jingquanhong/bruce-H-JEPA-in-World-Model/main/assets/videos/real_imu_forward.jpg">
          <source src="https://github.com/jingquanhong/bruce-H-JEPA-in-World-Model/raw/main/assets/videos/real_imu_forward.mp4" type="video/mp4">
        </video>
        <br/>
        <b>IMU 前进</b><br/>
        <sub>960×540 · 20.6 s · 30 fps</sub>
      </td>
      <td align="center" width="50%">
        <video width="380" controls preload="metadata"
          poster="https://raw.githubusercontent.com/jingquanhong/bruce-H-JEPA-in-World-Model/main/assets/videos/real_imu_backward.jpg">
          <source src="https://github.com/jingquanhong/bruce-H-JEPA-in-World-Model/raw/main/assets/videos/real_imu_backward.mp4" type="video/mp4">
        </video>
        <br/>
        <b>IMU 后退</b><br/>
        <sub>960×540 · 15.3 s · 29 fps</sub>
      </td>
    </tr>
  </table>
</div>

### 仿真：Genesis 越障采集

<div align="center">
  <table>
    <tr>
      <td align="center" width="50%">
        <video width="380" controls preload="metadata"
          poster="https://raw.githubusercontent.com/jingquanhong/bruce-H-JEPA-in-World-Model/main/assets/videos/sim_comparison.jpg">
          <source src="https://github.com/jingquanhong/bruce-H-JEPA-in-World-Model/raw/main/assets/videos/sim_comparison.mp4" type="video/mp4">
        </video>
        <br/>
        <b>基座辅助 vs 仅腿关节驱动</b><br/>
        <sub>分屏对比（失败，诚实呈现）</sub>
      </td>
      <td align="center" width="50%">
        <video width="380" controls preload="metadata"
          poster="https://raw.githubusercontent.com/jingquanhong/bruce-H-JEPA-in-World-Model/main/assets/videos/sim_stepover_8cm.jpg">
          <source src="https://github.com/jingquanhong/bruce-H-JEPA-in-World-Model/raw/main/assets/videos/sim_stepover_8cm.mp4" type="video/mp4">
        </video>
        <br/>
        <b>8 cm 障碍越障</b><br/>
        <sub>参考轨迹，非自主成功示范</sub>
      </td>
    </tr>
  </table>
</div>

| 模块 | 技术栈 |
|---|---|
| 仿真与采集 | Genesis · 100 Hz 记录 · 10 维腿关节动作 · 净空/踢箱/摔倒判定 |
| 信号保真 | 电流量化链（0.0333 A/LSB）· ±10.5 N·m 饱和 · IMU 比力 `Rᵀ(a+[0,0,g])` |
| 世界模型 | H-JEPA 分层 JEPA · `stable_worldmodel` HDF5 契约 · DROID 离线规划 |
| 实机工具链 | BRUCE-OP · 反馈健康门禁 · 单一执行者横移诊断 |

---

## 🔬 研究方向

- **人形机器人视觉语言导航（VLN）**：属性基元显式分解、姿态-代价耦合的极端路径评估
- **世界模型**：分层潜空间预测与规划，把物理复核嵌进每一步动作
- **零训练内推演**：拒绝强化学习试错，用可解析轨迹 + 物理约束替代试错采样

## 🛠️ 其他项目

| 方向 | 仓库 |
|---|---|
| 学术主页 | [PersonalPage](https://github.com/jingquanhong/PersonalPage) |
| RoboMaster 主控板 / M3508 底盘 | [rm_homework](https://github.com/jingquanhong/rm_homework) · [rm_m3508](https://github.com/jingquanhong/rm_m3508) |
| VEX 机器人 | [vex_skill](https://github.com/jingquanhong/vex_skill) · [vex_vision](https://github.com/jingquanhong/vex_vision) · [vexauto_add_geometry](https://github.com/jingquanhong/vexauto_add_geometry) |
| 救援与感知 | [earthquake_rescue_robot](https://github.com/jingquanhong/earthquake_rescue_robot) · [human_face_detect](https://github.com/jingquanhong/human_face_detect) |
| 其他 | [car-v3](https://github.com/jingquanhong/car-v3) · [simdog](https://github.com/jingquanhong/simdog) · [FreeBreathe](https://github.com/jingquanhong/FreeBreathe) |

---

<div align="center">

**主页**：<https://jingquanhong.github.io/Personal-Page/>

</div>
