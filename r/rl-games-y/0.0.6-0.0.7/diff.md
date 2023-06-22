# Comparing `tmp/rl_games_y-0.0.6.tar.gz` & `tmp/rl_games_y-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl_games_y-0.0.6.tar", max compression
+gzip compressed data, was "rl_games_y-0.0.7.tar", max compression
```

## Comparing `rl_games_y-0.0.6.tar` & `rl_games_y-0.0.7.tar`

### file list

```diff
@@ -1,234 +1,234 @@
--rw-r--r--   0        0        0     1068 2023-06-06 12:36:05.369197 rl_games_y-0.0.6/LICENSE
--rw-r--r--   0        0        0      104 2023-06-06 12:31:25.308716 rl_games_y-0.0.6/README.md
--rw-r--r--   0        0        0     1126 2023-06-20 13:50:51.624426 rl_games_y-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      414 2023-06-20 13:49:58.806735 rl_games_y-0.0.6/rl_games/.git/FETCH_HEAD
--rw-r--r--   0        0        0       29 2023-06-12 13:02:52.898759 rl_games_y-0.0.6/rl_games/.git/HEAD
--rw-r--r--   0        0        0       41 2023-06-20 13:49:58.814735 rl_games_y-0.0.6/rl_games/.git/ORIG_HEAD
--rw-r--r--   0        0        0      338 2023-06-12 13:02:52.898759 rl_games_y-0.0.6/rl_games/.git/config
--rw-r--r--   0        0        0       73 2023-06-06 12:22:19.330646 rl_games_y-0.0.6/rl_games/.git/description
--rwxr-xr-x   0        0        0      478 2023-06-06 12:22:19.330646 rl_games_y-0.0.6/rl_games/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0        0        0      896 2023-06-06 12:22:19.330646 rl_games_y-0.0.6/rl_games/.git/hooks/commit-msg.sample
--rwxr-xr-x   0        0        0     3079 2023-06-06 12:22:19.330646 rl_games_y-0.0.6/rl_games/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0        0        0      189 2023-06-06 12:22:19.330646 rl_games_y-0.0.6/rl_games/.git/hooks/post-update.sample
--rwxr-xr-x   0        0        0      424 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0        0        0     1638 2023-06-06 12:22:19.330646 rl_games_y-0.0.6/rl_games/.git/hooks/pre-commit.sample
--rwxr-xr-x   0        0        0      416 2023-06-06 12:22:19.330646 rl_games_y-0.0.6/rl_games/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0        0        0     1348 2023-06-06 12:22:19.330646 rl_games_y-0.0.6/rl_games/.git/hooks/pre-push.sample
--rwxr-xr-x   0        0        0     4898 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0        0        0      544 2023-06-06 12:22:19.330646 rl_games_y-0.0.6/rl_games/.git/hooks/pre-receive.sample
--rwxr-xr-x   0        0        0     1492 2023-06-06 12:22:19.330646 rl_games_y-0.0.6/rl_games/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0        0        0     3610 2023-06-06 12:22:19.330646 rl_games_y-0.0.6/rl_games/.git/hooks/update.sample
--rw-r--r--   0        0        0    17950 2023-06-20 13:50:02.090841 rl_games_y-0.0.6/rl_games/.git/index
--rw-r--r--   0        0        0      240 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/.git/info/exclude
--rw-r--r--   0        0        0     1214 2023-06-20 13:49:58.822736 rl_games_y-0.0.6/rl_games/.git/logs/HEAD
--rw-r--r--   0        0        0      858 2023-06-12 13:02:44.846532 rl_games_y-0.0.6/rl_games/.git/logs/refs/heads/master
--rw-r--r--   0        0        0      365 2023-06-20 13:49:58.826736 rl_games_y-0.0.6/rl_games/.git/logs/refs/heads/real_tfinger
--rw-r--r--   0        0        0      198 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/.git/logs/refs/remotes/origin/HEAD
--rw-r--r--   0        0        0      825 2023-06-20 13:49:58.798735 rl_games_y-0.0.6/rl_games/.git/logs/refs/remotes/origin/master
--rw-r--r--   0        0        0      330 2023-06-20 13:49:58.786734 rl_games_y-0.0.6/rl_games/.git/logs/refs/remotes/origin/real_tfinger
--rw-r--r--   0        0        0     1904 2023-06-12 11:46:56.868412 rl_games_y-0.0.6/rl_games/.git/objects/1b/8cb79243d15f5367053c2e0b6e08ee13486d2e
--rw-r--r--   0        0        0     1785 2023-06-20 13:49:58.766734 rl_games_y-0.0.6/rl_games/.git/objects/1f/721147f878fdca9c3b5dfdcf11fc4194427580
--rw-r--r--   0        0        0      177 2023-06-20 13:49:58.742733 rl_games_y-0.0.6/rl_games/.git/objects/43/3062580fc20427e1c30d4ce22237ae2f2b89d5
--rw-r--r--   0        0        0      195 2023-06-07 16:25:44.744437 rl_games_y-0.0.6/rl_games/.git/objects/4d/a9a4a73904107f7f059bd22e1801c86e340477
--rw-r--r--   0        0        0      353 2023-06-07 15:42:06.870977 rl_games_y-0.0.6/rl_games/.git/objects/5d/d72011a4c6b902c268b53c53c8c2603ffb1b24
--rw-r--r--   0        0        0      354 2023-06-20 13:49:58.754733 rl_games_y-0.0.6/rl_games/.git/objects/61/2da962b3da4292ee4fa9a108f7c5d299141544
--rw-r--r--   0        0        0      208 2023-06-12 13:02:44.758529 rl_games_y-0.0.6/rl_games/.git/objects/62/c29b659cb952ec70f1b9d5af60b7cbb0cca540
--rw-r--r--   0        0        0     2232 2023-06-20 13:49:58.766734 rl_games_y-0.0.6/rl_games/.git/objects/7e/42774f9165d4aa805bed4fe49a009ecd448cd8
--rw-r--r--   0        0        0      799 2023-06-07 16:25:44.748437 rl_games_y-0.0.6/rl_games/.git/objects/7e/f78f9e19649c9b3c47d1213b32250a9bf3e388
--rw-r--r--   0        0        0      799 2023-06-07 15:42:06.870977 rl_games_y-0.0.6/rl_games/.git/objects/83/9143ebf6fc1f117625473c0f843f5186fd5b4c
--rw-r--r--   0        0        0     3068 2023-06-07 16:25:44.748437 rl_games_y-0.0.6/rl_games/.git/objects/83/aec7354373d7b6c357a7a726955dd04e575b99
--rw-r--r--   0        0        0    11201 2023-06-20 13:49:58.766734 rl_games_y-0.0.6/rl_games/.git/objects/92/300cf5339afc007452ba03a6429fbac560beb7
--rw-r--r--   0        0        0      209 2023-06-20 13:49:58.754733 rl_games_y-0.0.6/rl_games/.git/objects/97/f9cf39e91a4d3ba0303f8d80f1bbf4bd791246
--rw-r--r--   0        0        0      354 2023-06-07 16:25:44.744437 rl_games_y-0.0.6/rl_games/.git/objects/ab/65a61e3067202668ed5e1a60fa5b99fce3d8fd
--rw-r--r--   0        0        0     2376 2023-06-12 11:46:56.868412 rl_games_y-0.0.6/rl_games/.git/objects/b0/53a46f62fd3debd26a8086221ba4b0b53da81e
--rw-r--r--   0        0        0      188 2023-06-07 15:42:06.870977 rl_games_y-0.0.6/rl_games/.git/objects/b2/9f1dc53920d5d037dc88b0a7b82e5fbabb3e84
--rw-r--r--   0        0        0      353 2023-06-12 11:46:56.852411 rl_games_y-0.0.6/rl_games/.git/objects/b9/1b35812c7f646d24a738815f4688bd622addb6
--rw-r--r--   0        0        0     3076 2023-06-07 15:42:06.874977 rl_games_y-0.0.6/rl_games/.git/objects/c5/83ed29df6ccd6f5b9a415df9d78cf577c922b6
--rw-r--r--   0        0        0    11535 2023-06-12 11:46:56.868412 rl_games_y-0.0.6/rl_games/.git/objects/c6/8117225b14532206c1fdab9afc9c7f164587cb
--rw-r--r--   0        0        0      201 2023-06-12 11:46:56.852411 rl_games_y-0.0.6/rl_games/.git/objects/cd/c2e9da476a5be6b970127ca71ddce8432f2ba5
--rw-r--r--   0        0        0      581 2023-06-20 13:49:58.762734 rl_games_y-0.0.6/rl_games/.git/objects/ea/7ad0bc4ca97b0bb110ea383d1885f5d4e512e2
--rw-r--r--   0        0        0      580 2023-06-12 11:46:56.852411 rl_games_y-0.0.6/rl_games/.git/objects/f9/b97cccad3a3e540b8be03cc28da412957084ad
--rw-r--r--   0        0        0    11936 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.idx
--rw-r--r--   0        0        0   210728 2023-06-20 13:49:58.000000 rl_games_y-0.0.6/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.pack
--rw-r--r--   0        0        0      247 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/.git/packed-refs
--rw-r--r--   0        0        0       41 2023-06-12 13:02:44.846532 rl_games_y-0.0.6/rl_games/.git/refs/heads/master
--rw-r--r--   0        0        0       41 2023-06-20 13:49:58.822736 rl_games_y-0.0.6/rl_games/.git/refs/heads/real_tfinger
--rw-r--r--   0        0        0       32 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/.git/refs/remotes/origin/HEAD
--rw-r--r--   0        0        0       41 2023-06-20 13:49:58.798735 rl_games_y-0.0.6/rl_games/.git/refs/remotes/origin/master
--rw-r--r--   0        0        0       41 2023-06-20 13:49:58.786734 rl_games_y-0.0.6/rl_games/.git/refs/remotes/origin/real_tfinger
--rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/algos_torch/__init__.py
--rw-r--r--   0        0        0     8605 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/algos_torch/a2c_continuous.py
--rw-r--r--   0        0        0     7125 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/algos_torch/a2c_discrete.py
--rw-r--r--   0        0        0    10679 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/algos_torch/central_value.py
--rw-r--r--   0        0        0     1259 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/algos_torch/d2rl.py
--rw-r--r--   0        0        0    10830 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/algos_torch/flatten.py
--rw-r--r--   0        0        0     4148 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/algos_torch/layers.py
--rw-r--r--   0        0        0     2886 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/algos_torch/model_builder.py
--rw-r--r--   0        0        0    12119 2023-06-20 13:49:58.818735 rl_games_y-0.0.6/rl_games/algos_torch/models.py
--rw-r--r--   0        0        0     2729 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/algos_torch/moving_mean_std.py
--rw-r--r--   0        0        0    57650 2023-06-20 13:49:58.818735 rl_games_y-0.0.6/rl_games/algos_torch/network_builder.py
--rw-r--r--   0        0        0     8067 2023-06-20 13:49:58.822736 rl_games_y-0.0.6/rl_games/algos_torch/players.py
--rw-r--r--   0        0        0     4111 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/algos_torch/running_mean_std.py
--rw-r--r--   0        0        0    23967 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/algos_torch/sac_agent.py
--rw-r--r--   0        0        0     1618 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/algos_torch/sac_helper.py
--rw-r--r--   0        0        0     1332 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/algos_torch/self_play_manager.py
--rw-r--r--   0        0        0    12758 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/algos_torch/torch_ext.py
--rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/__init__.py
--rw-r--r--   0        0        0    55205 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/a2c_common.py
--rw-r--r--   0        0        0     5456 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/algo_observer.py
--rw-r--r--   0        0        0     1977 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/categorical.py
--rw-r--r--   0        0        0     2255 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/common_losses.py
--rw-r--r--   0        0        0     3396 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/datasets.py
--rw-r--r--   0        0        0     2284 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/diagnostics.py
--rw-r--r--   0        0        0      680 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/divergence.py
--rw-r--r--   0        0        0    15196 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/env_configurations.py
--rw-r--r--   0        0        0    17184 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/experience.py
--rw-r--r--   0        0        0     2440 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/experiment.py
--rw-r--r--   0        0        0     2750 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/interval_summary_writer.py
--rw-r--r--   0        0        0      945 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/ivecenv.py
--rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/layers/__init__.py
--rw-r--r--   0        0        0     2763 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/layers/recurrent.py
--rw-r--r--   0        0        0      414 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/object_factory.py
--rw-r--r--   0        0        0    10939 2023-06-12 13:02:52.898759 rl_games_y-0.0.6/rl_games/common/player.py
--rw-r--r--   0        0        0      382 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/rollouts.py
--rw-r--r--   0        0        0     1948 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/schedulers.py
--rw-r--r--   0        0        0     4888 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/segment_tree.py
--rw-r--r--   0        0        0     2260 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/tr_helpers.py
--rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/transforms/__init__.py
--rw-r--r--   0        0        0     1165 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/transforms/soft_augmentation.py
--rw-r--r--   0        0        0      746 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/transforms/transforms.py
--rw-r--r--   0        0        0     8191 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/vecenv.py
--rw-r--r--   0        0        0    23776 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/common/wrappers.py
--rw-r--r--   0        0        0     1606 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_breakout.yaml
--rw-r--r--   0        0        0     1545 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_breakout_envpool.yaml
--rw-r--r--   0        0        0     1468 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_breakout_envpool_resnet.yaml
--rw-r--r--   0        0        0     1380 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_breakout_torch_impala.yaml
--rw-r--r--   0        0        0     1607 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_gopher.yaml
--rw-r--r--   0        0        0     1688 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_invaders_envpool.yaml
--rw-r--r--   0        0        0     1834 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_invaders_envpool_rnn.yaml
--rw-r--r--   0        0        0     1730 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_pacman_envpool.yaml
--rw-r--r--   0        0        0     1518 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_pacman_envpool_resnet.yaml
--rw-r--r--   0        0        0     1841 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_pacman_envpool_rnn.yaml
--rw-r--r--   0        0        0     1619 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_pacman_torch.yaml
--rw-r--r--   0        0        0     1729 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_pacman_torch_rnn.yaml
--rw-r--r--   0        0        0     1650 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_pong.yaml
--rw-r--r--   0        0        0     1618 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_pong_envpool.yaml
--rw-r--r--   0        0        0     1434 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_pong_envpool_resnet.yaml
--rw-r--r--   0        0        0     1334 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_space_invaders_resnet.yaml
--rw-r--r--   0        0        0     1640 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/atari/ppo_space_invaders_torch.yaml
--rw-r--r--   0        0        0     1315 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/brax/ppo_ant.yaml
--rw-r--r--   0        0        0     1029 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/brax/ppo_ant_tcnn.yaml
--rw-r--r--   0        0        0     1264 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/brax/ppo_grasp.yaml
--rw-r--r--   0        0        0     1273 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/brax/ppo_halfcheetah.yaml
--rw-r--r--   0        0        0     1344 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/brax/ppo_humanoid.yaml
--rw-r--r--   0        0        0     1260 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/brax/ppo_ur5e.yaml
--rw-r--r--   0        0        0      902 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/brax/sac_ant.yaml
--rw-r--r--   0        0        0      904 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/brax/sac_humanoid.yaml
--rw-r--r--   0        0        0     1651 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/carracing_ppo.yaml
--rw-r--r--   0        0        0     1129 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/dm_control/cartpole.yaml
--rw-r--r--   0        0        0     1339 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/dm_control/fish_swim.yaml
--rw-r--r--   0        0        0     1280 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/dm_control/humanoid_run.yaml
--rw-r--r--   0        0        0     1239 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/dm_control/walker_run.yaml
--rw-r--r--   0        0        0     1226 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/dm_control/walker_stand.yaml
--rw-r--r--   0        0        0     1280 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/dm_control/walker_walk.yaml
--rw-r--r--   0        0        0     1660 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ma/ppo_connect4_self_play.yaml
--rw-r--r--   0        0        0      978 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ma/ppo_connect4_self_play_resnet.yaml
--rw-r--r--   0        0        0     1221 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ma/ppo_slime_self_play.yaml
--rw-r--r--   0        0        0     1029 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ma/ppo_slime_v0.yaml
--rw-r--r--   0        0        0     1744 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/minigrid/lava_rnn_img.yaml
--rw-r--r--   0        0        0     1688 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/minigrid/minigrid_rnn_img.yaml
--rw-r--r--   0        0        0     1209 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/mujoco/ant.yaml
--rw-r--r--   0        0        0     1245 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/mujoco/ant_envpool.yaml
--rw-r--r--   0        0        0     1276 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/mujoco/halfcheetah.yaml
--rw-r--r--   0        0        0     1351 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/mujoco/halfcheetah_envpool.yaml
--rw-r--r--   0        0        0     1242 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/mujoco/hopper.yaml
--rw-r--r--   0        0        0     1268 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/mujoco/hopper_envpool.yaml
--rw-r--r--   0        0        0     1290 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/mujoco/humanoid.yaml
--rw-r--r--   0        0        0     1279 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/mujoco/humanoid_envpool.yaml
--rw-r--r--   0        0        0      828 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/mujoco/sac_ant_envpool.yaml
--rw-r--r--   0        0        0      913 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/mujoco/sac_halfcheetah_envpool.yaml
--rw-r--r--   0        0        0     1196 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/mujoco/walker2d.yaml
--rw-r--r--   0        0        0     1228 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/mujoco/walker2d_envpool.yaml
--rw-r--r--   0        0        0     1223 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/openai/ppo_gym_ant.yaml
--rw-r--r--   0        0        0     1266 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/openai/ppo_gym_hand.yaml
--rw-r--r--   0        0        0     1226 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/openai/ppo_gym_humanoid.yaml
--rw-r--r--   0        0        0      907 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_cartpole.yaml
--rw-r--r--   0        0        0     1103 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_cartpole_masked_velocity_rnn.yaml
--rw-r--r--   0        0        0     1251 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_continuous.yaml
--rw-r--r--   0        0        0     1190 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_continuous_lstm.yaml
--rw-r--r--   0        0        0     1234 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_lunar.yaml
--rw-r--r--   0        0        0     1178 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_lunar_continiuos_torch.yaml
--rw-r--r--   0        0        0      868 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_lunar_discrete.yaml
--rw-r--r--   0        0        0     1723 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_multiwalker.yaml
--rw-r--r--   0        0        0     1159 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_pendulum.yaml
--rw-r--r--   0        0        0     1128 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_pendulum_torch.yaml
--rw-r--r--   0        0        0     1508 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_reacher.yaml
--rw-r--r--   0        0        0      905 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_smac.yaml
--rw-r--r--   0        0        0     1303 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_walker.yaml
--rw-r--r--   0        0        0     1258 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_walker_hardcore.yaml
--rw-r--r--   0        0        0     1483 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_walker_rnn.yaml
--rw-r--r--   0        0        0     1081 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/ppo_walker_tcnn.yaml
--rw-r--r--   0        0        0     1219 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/procgen/ppo_coinrun.yaml
--rw-r--r--   0        0        0     1379 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/10m_vs_11m_torch.yaml
--rw-r--r--   0        0        0     1709 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/27m_vs_30m_cv.yaml
--rw-r--r--   0        0        0     1380 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/27m_vs_30m_torch.yaml
--rw-r--r--   0        0        0      904 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/2m_vs_1z.yaml
--rw-r--r--   0        0        0      910 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/2m_vs_1z_torch.yaml
--rw-r--r--   0        0        0      966 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/2s_vs_1c.yaml
--rw-r--r--   0        0        0     1443 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/3m_cnn_torch.yaml
--rw-r--r--   0        0        0      956 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/3m_torch.yaml
--rw-r--r--   0        0        0     1470 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/3m_torch_cv.yaml
--rw-r--r--   0        0        0     1644 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/3m_torch_cv_joint.yaml
--rw-r--r--   0        0        0     1647 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/3m_torch_cv_rnn.yaml
--rw-r--r--   0        0        0     1037 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/3m_torch_rnn.yaml
--rw-r--r--   0        0        0     1545 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/3m_torch_sparse.yaml
--rw-r--r--   0        0        0     1516 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/3s5z_vs_3s6z_torch.yaml
--rw-r--r--   0        0        0     1520 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/3s5z_vs_3s6z_torch_cv.yaml
--rw-r--r--   0        0        0      961 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/3s_vs_4z.yaml
--rw-r--r--   0        0        0      970 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/3s_vs_5z.yaml
--rw-r--r--   0        0        0     1473 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/3s_vs_5z_cv.yaml
--rw-r--r--   0        0        0     1681 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/3s_vs_5z_cv_rnn.yaml
--rw-r--r--   0        0        0     1047 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/3s_vs_5z_torch_lstm.yaml
--rw-r--r--   0        0        0     1022 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/3s_vs_5z_torch_lstm2.yaml
--rw-r--r--   0        0        0     1287 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/5m_vs_6m_rnn.yaml
--rw-r--r--   0        0        0     1883 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/5m_vs_6m_rnn_cv.yaml
--rw-r--r--   0        0        0     1437 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/5m_vs_6m_torch.yaml
--rw-r--r--   0        0        0     1043 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/6h_vs_8z_torch.yaml
--rw-r--r--   0        0        0     1669 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/6h_vs_8z_torch_cv.yaml
--rw-r--r--   0        0        0      993 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/8m_torch.yaml
--rw-r--r--   0        0        0     1509 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/8m_torch_cv.yaml
--rw-r--r--   0        0        0     1457 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/MMM2_torch.yaml
--rw-r--r--   0        0        0     1456 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/corridor_torch.yaml
--rw-r--r--   0        0        0     1515 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/smac/corridor_torch_cv.yaml
--rw-r--r--   0        0        0     1965 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/test/test_asymmetric_continuous.yaml
--rw-r--r--   0        0        0     1712 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/test/test_asymmetric_discrete.yaml
--rw-r--r--   0        0        0     1873 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/test/test_asymmetric_discrete_mhv.yaml
--rw-r--r--   0        0        0     1401 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/test/test_asymmetric_discrete_mhv_mops.yaml
--rw-r--r--   0        0        0     1146 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/test/test_discrete.yaml
--rw-r--r--   0        0        0     1162 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/test/test_discrete_multidiscrete_mhv.yaml
--rw-r--r--   0        0        0     1301 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/test/test_ppo_walker_truncated_time.yaml
--rw-r--r--   0        0        0     1205 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/test/test_rnn.yaml
--rw-r--r--   0        0        0     1829 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/test/test_rnn_multidiscrete.yaml
--rw-r--r--   0        0        0     1325 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/configs/test/test_rnn_multidiscrete_mhv.yaml
--rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/distributed/__init__.py
--rw-r--r--   0        0        0      281 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/envs/__init__.py
--rw-r--r--   0        0        0     1941 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/envs/brax.py
--rw-r--r--   0        0        0     2992 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/envs/connect4_network.py
--rw-r--r--   0        0        0     4505 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/envs/connect4_selfplay.py
--rw-r--r--   0        0        0     3496 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/envs/diambra/diambra.py
--rw-r--r--   0        0        0     3116 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/envs/envpool.py
--rw-r--r--   0        0        0     3195 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/envs/multiwalker.py
--rw-r--r--   0        0        0     2148 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/envs/slimevolley_selfplay.py
--rw-r--r--   0        0        0     3690 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/envs/smac_env.py
--rw-r--r--   0        0        0      279 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/envs/test/__init__.py
--rw-r--r--   0        0        0      779 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/envs/test/example_env.py
--rw-r--r--   0        0        0     5217 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/envs/test/rnn_env.py
--rw-r--r--   0        0        0     1715 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/envs/test/test_asymmetric_env.py
--rw-r--r--   0        0        0     1596 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/envs/test_network.py
--rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/interfaces/__init__.py
--rw-r--r--   0        0        0      674 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/interfaces/base_algorithm.py
--rw-r--r--   0        0        0      159 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/networks/__init__.py
--rw-r--r--   0        0        0     1463 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/networks/tcnn_mlp.py
--rw-r--r--   0        0        0     4860 2023-06-06 12:22:19.334646 rl_games_y-0.0.6/rl_games/torch_runner.py
--rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 rl_games_y-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-06 12:36:05.369197 rl_games_y-0.0.7/LICENSE
+-rw-r--r--   0        0        0      104 2023-06-06 12:31:25.308716 rl_games_y-0.0.7/README.md
+-rw-r--r--   0        0        0     1126 2023-06-22 12:06:58.133718 rl_games_y-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      414 2023-06-20 13:49:58.806735 rl_games_y-0.0.7/rl_games/.git/FETCH_HEAD
+-rw-r--r--   0        0        0       29 2023-06-12 13:02:52.898759 rl_games_y-0.0.7/rl_games/.git/HEAD
+-rw-r--r--   0        0        0       41 2023-06-20 13:49:58.814735 rl_games_y-0.0.7/rl_games/.git/ORIG_HEAD
+-rw-r--r--   0        0        0      338 2023-06-12 13:02:52.898759 rl_games_y-0.0.7/rl_games/.git/config
+-rw-r--r--   0        0        0       73 2023-06-06 12:22:19.330646 rl_games_y-0.0.7/rl_games/.git/description
+-rwxr-xr-x   0        0        0      478 2023-06-06 12:22:19.330646 rl_games_y-0.0.7/rl_games/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0        0        0      896 2023-06-06 12:22:19.330646 rl_games_y-0.0.7/rl_games/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0        0        0     3079 2023-06-06 12:22:19.330646 rl_games_y-0.0.7/rl_games/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0        0        0      189 2023-06-06 12:22:19.330646 rl_games_y-0.0.7/rl_games/.git/hooks/post-update.sample
+-rwxr-xr-x   0        0        0      424 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0        0        0     1638 2023-06-06 12:22:19.330646 rl_games_y-0.0.7/rl_games/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0        0        0      416 2023-06-06 12:22:19.330646 rl_games_y-0.0.7/rl_games/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0        0        0     1348 2023-06-06 12:22:19.330646 rl_games_y-0.0.7/rl_games/.git/hooks/pre-push.sample
+-rwxr-xr-x   0        0        0     4898 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0        0        0      544 2023-06-06 12:22:19.330646 rl_games_y-0.0.7/rl_games/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0        0        0     1492 2023-06-06 12:22:19.330646 rl_games_y-0.0.7/rl_games/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0        0        0     3610 2023-06-06 12:22:19.330646 rl_games_y-0.0.7/rl_games/.git/hooks/update.sample
+-rw-r--r--   0        0        0    17950 2023-06-20 13:50:02.090841 rl_games_y-0.0.7/rl_games/.git/index
+-rw-r--r--   0        0        0      240 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/.git/info/exclude
+-rw-r--r--   0        0        0     1214 2023-06-20 13:49:58.822736 rl_games_y-0.0.7/rl_games/.git/logs/HEAD
+-rw-r--r--   0        0        0      858 2023-06-12 13:02:44.846532 rl_games_y-0.0.7/rl_games/.git/logs/refs/heads/master
+-rw-r--r--   0        0        0      365 2023-06-20 13:49:58.826736 rl_games_y-0.0.7/rl_games/.git/logs/refs/heads/real_tfinger
+-rw-r--r--   0        0        0      198 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/.git/logs/refs/remotes/origin/HEAD
+-rw-r--r--   0        0        0      825 2023-06-20 13:49:58.798735 rl_games_y-0.0.7/rl_games/.git/logs/refs/remotes/origin/master
+-rw-r--r--   0        0        0      330 2023-06-20 13:49:58.786734 rl_games_y-0.0.7/rl_games/.git/logs/refs/remotes/origin/real_tfinger
+-rw-r--r--   0        0        0     1904 2023-06-12 11:46:56.868412 rl_games_y-0.0.7/rl_games/.git/objects/1b/8cb79243d15f5367053c2e0b6e08ee13486d2e
+-rw-r--r--   0        0        0     1785 2023-06-20 13:49:58.766734 rl_games_y-0.0.7/rl_games/.git/objects/1f/721147f878fdca9c3b5dfdcf11fc4194427580
+-rw-r--r--   0        0        0      177 2023-06-20 13:49:58.742733 rl_games_y-0.0.7/rl_games/.git/objects/43/3062580fc20427e1c30d4ce22237ae2f2b89d5
+-rw-r--r--   0        0        0      195 2023-06-07 16:25:44.744437 rl_games_y-0.0.7/rl_games/.git/objects/4d/a9a4a73904107f7f059bd22e1801c86e340477
+-rw-r--r--   0        0        0      353 2023-06-07 15:42:06.870977 rl_games_y-0.0.7/rl_games/.git/objects/5d/d72011a4c6b902c268b53c53c8c2603ffb1b24
+-rw-r--r--   0        0        0      354 2023-06-20 13:49:58.754733 rl_games_y-0.0.7/rl_games/.git/objects/61/2da962b3da4292ee4fa9a108f7c5d299141544
+-rw-r--r--   0        0        0      208 2023-06-12 13:02:44.758529 rl_games_y-0.0.7/rl_games/.git/objects/62/c29b659cb952ec70f1b9d5af60b7cbb0cca540
+-rw-r--r--   0        0        0     2232 2023-06-20 13:49:58.766734 rl_games_y-0.0.7/rl_games/.git/objects/7e/42774f9165d4aa805bed4fe49a009ecd448cd8
+-rw-r--r--   0        0        0      799 2023-06-07 16:25:44.748437 rl_games_y-0.0.7/rl_games/.git/objects/7e/f78f9e19649c9b3c47d1213b32250a9bf3e388
+-rw-r--r--   0        0        0      799 2023-06-07 15:42:06.870977 rl_games_y-0.0.7/rl_games/.git/objects/83/9143ebf6fc1f117625473c0f843f5186fd5b4c
+-rw-r--r--   0        0        0     3068 2023-06-07 16:25:44.748437 rl_games_y-0.0.7/rl_games/.git/objects/83/aec7354373d7b6c357a7a726955dd04e575b99
+-rw-r--r--   0        0        0    11201 2023-06-20 13:49:58.766734 rl_games_y-0.0.7/rl_games/.git/objects/92/300cf5339afc007452ba03a6429fbac560beb7
+-rw-r--r--   0        0        0      209 2023-06-20 13:49:58.754733 rl_games_y-0.0.7/rl_games/.git/objects/97/f9cf39e91a4d3ba0303f8d80f1bbf4bd791246
+-rw-r--r--   0        0        0      354 2023-06-07 16:25:44.744437 rl_games_y-0.0.7/rl_games/.git/objects/ab/65a61e3067202668ed5e1a60fa5b99fce3d8fd
+-rw-r--r--   0        0        0     2376 2023-06-12 11:46:56.868412 rl_games_y-0.0.7/rl_games/.git/objects/b0/53a46f62fd3debd26a8086221ba4b0b53da81e
+-rw-r--r--   0        0        0      188 2023-06-07 15:42:06.870977 rl_games_y-0.0.7/rl_games/.git/objects/b2/9f1dc53920d5d037dc88b0a7b82e5fbabb3e84
+-rw-r--r--   0        0        0      353 2023-06-12 11:46:56.852411 rl_games_y-0.0.7/rl_games/.git/objects/b9/1b35812c7f646d24a738815f4688bd622addb6
+-rw-r--r--   0        0        0     3076 2023-06-07 15:42:06.874977 rl_games_y-0.0.7/rl_games/.git/objects/c5/83ed29df6ccd6f5b9a415df9d78cf577c922b6
+-rw-r--r--   0        0        0    11535 2023-06-12 11:46:56.868412 rl_games_y-0.0.7/rl_games/.git/objects/c6/8117225b14532206c1fdab9afc9c7f164587cb
+-rw-r--r--   0        0        0      201 2023-06-12 11:46:56.852411 rl_games_y-0.0.7/rl_games/.git/objects/cd/c2e9da476a5be6b970127ca71ddce8432f2ba5
+-rw-r--r--   0        0        0      581 2023-06-20 13:49:58.762734 rl_games_y-0.0.7/rl_games/.git/objects/ea/7ad0bc4ca97b0bb110ea383d1885f5d4e512e2
+-rw-r--r--   0        0        0      580 2023-06-12 11:46:56.852411 rl_games_y-0.0.7/rl_games/.git/objects/f9/b97cccad3a3e540b8be03cc28da412957084ad
+-rw-r--r--   0        0        0    11936 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.idx
+-rw-r--r--   0        0        0   210728 2023-06-20 13:49:58.000000 rl_games_y-0.0.7/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.pack
+-rw-r--r--   0        0        0      247 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/.git/packed-refs
+-rw-r--r--   0        0        0       41 2023-06-12 13:02:44.846532 rl_games_y-0.0.7/rl_games/.git/refs/heads/master
+-rw-r--r--   0        0        0       41 2023-06-20 13:49:58.822736 rl_games_y-0.0.7/rl_games/.git/refs/heads/real_tfinger
+-rw-r--r--   0        0        0       32 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/.git/refs/remotes/origin/HEAD
+-rw-r--r--   0        0        0       41 2023-06-20 13:49:58.798735 rl_games_y-0.0.7/rl_games/.git/refs/remotes/origin/master
+-rw-r--r--   0        0        0       41 2023-06-20 13:49:58.786734 rl_games_y-0.0.7/rl_games/.git/refs/remotes/origin/real_tfinger
+-rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/algos_torch/__init__.py
+-rw-r--r--   0        0        0     8605 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/algos_torch/a2c_continuous.py
+-rw-r--r--   0        0        0     7125 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/algos_torch/a2c_discrete.py
+-rw-r--r--   0        0        0    10679 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/algos_torch/central_value.py
+-rw-r--r--   0        0        0     1259 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/algos_torch/d2rl.py
+-rw-r--r--   0        0        0    10830 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/algos_torch/flatten.py
+-rw-r--r--   0        0        0     4148 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/algos_torch/layers.py
+-rw-r--r--   0        0        0     2886 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/algos_torch/model_builder.py
+-rw-r--r--   0        0        0    12119 2023-06-20 13:49:58.818735 rl_games_y-0.0.7/rl_games/algos_torch/models.py
+-rw-r--r--   0        0        0     2729 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/algos_torch/moving_mean_std.py
+-rw-r--r--   0        0        0    57650 2023-06-20 13:49:58.818735 rl_games_y-0.0.7/rl_games/algos_torch/network_builder.py
+-rw-r--r--   0        0        0     8067 2023-06-20 13:49:58.822736 rl_games_y-0.0.7/rl_games/algos_torch/players.py
+-rw-r--r--   0        0        0     4111 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/algos_torch/running_mean_std.py
+-rw-r--r--   0        0        0    23967 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/algos_torch/sac_agent.py
+-rw-r--r--   0        0        0     1618 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/algos_torch/sac_helper.py
+-rw-r--r--   0        0        0     1332 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/algos_torch/self_play_manager.py
+-rw-r--r--   0        0        0    12758 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/algos_torch/torch_ext.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/__init__.py
+-rw-r--r--   0        0        0    55205 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/a2c_common.py
+-rw-r--r--   0        0        0     5456 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/algo_observer.py
+-rw-r--r--   0        0        0     1977 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/categorical.py
+-rw-r--r--   0        0        0     2255 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/common_losses.py
+-rw-r--r--   0        0        0     3396 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/datasets.py
+-rw-r--r--   0        0        0     2284 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/diagnostics.py
+-rw-r--r--   0        0        0      680 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/divergence.py
+-rw-r--r--   0        0        0    15196 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/env_configurations.py
+-rw-r--r--   0        0        0    17184 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/experience.py
+-rw-r--r--   0        0        0     2440 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/experiment.py
+-rw-r--r--   0        0        0     2750 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/interval_summary_writer.py
+-rw-r--r--   0        0        0      945 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/ivecenv.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/layers/__init__.py
+-rw-r--r--   0        0        0     2763 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/layers/recurrent.py
+-rw-r--r--   0        0        0      414 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/object_factory.py
+-rw-r--r--   0        0        0    10939 2023-06-12 13:02:52.898759 rl_games_y-0.0.7/rl_games/common/player.py
+-rw-r--r--   0        0        0      382 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/rollouts.py
+-rw-r--r--   0        0        0     1948 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/schedulers.py
+-rw-r--r--   0        0        0     4888 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/segment_tree.py
+-rw-r--r--   0        0        0     2260 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/tr_helpers.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/transforms/__init__.py
+-rw-r--r--   0        0        0     1165 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/transforms/soft_augmentation.py
+-rw-r--r--   0        0        0      746 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/transforms/transforms.py
+-rw-r--r--   0        0        0     8191 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/vecenv.py
+-rw-r--r--   0        0        0    23776 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/common/wrappers.py
+-rw-r--r--   0        0        0     1606 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_breakout.yaml
+-rw-r--r--   0        0        0     1545 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_breakout_envpool.yaml
+-rw-r--r--   0        0        0     1468 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_breakout_envpool_resnet.yaml
+-rw-r--r--   0        0        0     1380 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_breakout_torch_impala.yaml
+-rw-r--r--   0        0        0     1607 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_gopher.yaml
+-rw-r--r--   0        0        0     1688 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_invaders_envpool.yaml
+-rw-r--r--   0        0        0     1834 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_invaders_envpool_rnn.yaml
+-rw-r--r--   0        0        0     1730 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_pacman_envpool.yaml
+-rw-r--r--   0        0        0     1518 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_pacman_envpool_resnet.yaml
+-rw-r--r--   0        0        0     1841 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_pacman_envpool_rnn.yaml
+-rw-r--r--   0        0        0     1619 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_pacman_torch.yaml
+-rw-r--r--   0        0        0     1729 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_pacman_torch_rnn.yaml
+-rw-r--r--   0        0        0     1650 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_pong.yaml
+-rw-r--r--   0        0        0     1618 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_pong_envpool.yaml
+-rw-r--r--   0        0        0     1434 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_pong_envpool_resnet.yaml
+-rw-r--r--   0        0        0     1334 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_space_invaders_resnet.yaml
+-rw-r--r--   0        0        0     1640 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/atari/ppo_space_invaders_torch.yaml
+-rw-r--r--   0        0        0     1315 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/brax/ppo_ant.yaml
+-rw-r--r--   0        0        0     1029 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/brax/ppo_ant_tcnn.yaml
+-rw-r--r--   0        0        0     1264 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/brax/ppo_grasp.yaml
+-rw-r--r--   0        0        0     1273 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/brax/ppo_halfcheetah.yaml
+-rw-r--r--   0        0        0     1344 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/brax/ppo_humanoid.yaml
+-rw-r--r--   0        0        0     1260 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/brax/ppo_ur5e.yaml
+-rw-r--r--   0        0        0      902 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/brax/sac_ant.yaml
+-rw-r--r--   0        0        0      904 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/brax/sac_humanoid.yaml
+-rw-r--r--   0        0        0     1651 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/carracing_ppo.yaml
+-rw-r--r--   0        0        0     1129 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/dm_control/cartpole.yaml
+-rw-r--r--   0        0        0     1339 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/dm_control/fish_swim.yaml
+-rw-r--r--   0        0        0     1280 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/dm_control/humanoid_run.yaml
+-rw-r--r--   0        0        0     1239 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/dm_control/walker_run.yaml
+-rw-r--r--   0        0        0     1226 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/dm_control/walker_stand.yaml
+-rw-r--r--   0        0        0     1280 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/dm_control/walker_walk.yaml
+-rw-r--r--   0        0        0     1660 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ma/ppo_connect4_self_play.yaml
+-rw-r--r--   0        0        0      978 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ma/ppo_connect4_self_play_resnet.yaml
+-rw-r--r--   0        0        0     1221 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ma/ppo_slime_self_play.yaml
+-rw-r--r--   0        0        0     1029 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ma/ppo_slime_v0.yaml
+-rw-r--r--   0        0        0     1744 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/minigrid/lava_rnn_img.yaml
+-rw-r--r--   0        0        0     1688 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/minigrid/minigrid_rnn_img.yaml
+-rw-r--r--   0        0        0     1209 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/mujoco/ant.yaml
+-rw-r--r--   0        0        0     1245 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/mujoco/ant_envpool.yaml
+-rw-r--r--   0        0        0     1276 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/mujoco/halfcheetah.yaml
+-rw-r--r--   0        0        0     1351 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/mujoco/halfcheetah_envpool.yaml
+-rw-r--r--   0        0        0     1242 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/mujoco/hopper.yaml
+-rw-r--r--   0        0        0     1268 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/mujoco/hopper_envpool.yaml
+-rw-r--r--   0        0        0     1290 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/mujoco/humanoid.yaml
+-rw-r--r--   0        0        0     1279 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/mujoco/humanoid_envpool.yaml
+-rw-r--r--   0        0        0      828 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/mujoco/sac_ant_envpool.yaml
+-rw-r--r--   0        0        0      913 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/mujoco/sac_halfcheetah_envpool.yaml
+-rw-r--r--   0        0        0     1196 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/mujoco/walker2d.yaml
+-rw-r--r--   0        0        0     1228 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/mujoco/walker2d_envpool.yaml
+-rw-r--r--   0        0        0     1223 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/openai/ppo_gym_ant.yaml
+-rw-r--r--   0        0        0     1266 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/openai/ppo_gym_hand.yaml
+-rw-r--r--   0        0        0     1226 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/openai/ppo_gym_humanoid.yaml
+-rw-r--r--   0        0        0      907 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_cartpole.yaml
+-rw-r--r--   0        0        0     1103 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_cartpole_masked_velocity_rnn.yaml
+-rw-r--r--   0        0        0     1251 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_continuous.yaml
+-rw-r--r--   0        0        0     1190 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_continuous_lstm.yaml
+-rw-r--r--   0        0        0     1234 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_lunar.yaml
+-rw-r--r--   0        0        0     1178 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_lunar_continiuos_torch.yaml
+-rw-r--r--   0        0        0      868 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_lunar_discrete.yaml
+-rw-r--r--   0        0        0     1723 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_multiwalker.yaml
+-rw-r--r--   0        0        0     1159 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_pendulum.yaml
+-rw-r--r--   0        0        0     1128 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_pendulum_torch.yaml
+-rw-r--r--   0        0        0     1508 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_reacher.yaml
+-rw-r--r--   0        0        0      905 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_smac.yaml
+-rw-r--r--   0        0        0     1303 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_walker.yaml
+-rw-r--r--   0        0        0     1258 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_walker_hardcore.yaml
+-rw-r--r--   0        0        0     1483 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_walker_rnn.yaml
+-rw-r--r--   0        0        0     1081 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/ppo_walker_tcnn.yaml
+-rw-r--r--   0        0        0     1219 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/procgen/ppo_coinrun.yaml
+-rw-r--r--   0        0        0     1379 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/10m_vs_11m_torch.yaml
+-rw-r--r--   0        0        0     1709 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/27m_vs_30m_cv.yaml
+-rw-r--r--   0        0        0     1380 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/27m_vs_30m_torch.yaml
+-rw-r--r--   0        0        0      904 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/2m_vs_1z.yaml
+-rw-r--r--   0        0        0      910 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/2m_vs_1z_torch.yaml
+-rw-r--r--   0        0        0      966 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/2s_vs_1c.yaml
+-rw-r--r--   0        0        0     1443 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/3m_cnn_torch.yaml
+-rw-r--r--   0        0        0      956 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/3m_torch.yaml
+-rw-r--r--   0        0        0     1470 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/3m_torch_cv.yaml
+-rw-r--r--   0        0        0     1644 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/3m_torch_cv_joint.yaml
+-rw-r--r--   0        0        0     1647 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/3m_torch_cv_rnn.yaml
+-rw-r--r--   0        0        0     1037 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/3m_torch_rnn.yaml
+-rw-r--r--   0        0        0     1545 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/3m_torch_sparse.yaml
+-rw-r--r--   0        0        0     1516 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/3s5z_vs_3s6z_torch.yaml
+-rw-r--r--   0        0        0     1520 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/3s5z_vs_3s6z_torch_cv.yaml
+-rw-r--r--   0        0        0      961 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/3s_vs_4z.yaml
+-rw-r--r--   0        0        0      970 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/3s_vs_5z.yaml
+-rw-r--r--   0        0        0     1473 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/3s_vs_5z_cv.yaml
+-rw-r--r--   0        0        0     1681 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/3s_vs_5z_cv_rnn.yaml
+-rw-r--r--   0        0        0     1047 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/3s_vs_5z_torch_lstm.yaml
+-rw-r--r--   0        0        0     1022 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/3s_vs_5z_torch_lstm2.yaml
+-rw-r--r--   0        0        0     1287 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/5m_vs_6m_rnn.yaml
+-rw-r--r--   0        0        0     1883 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/5m_vs_6m_rnn_cv.yaml
+-rw-r--r--   0        0        0     1437 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/5m_vs_6m_torch.yaml
+-rw-r--r--   0        0        0     1043 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/6h_vs_8z_torch.yaml
+-rw-r--r--   0        0        0     1669 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/6h_vs_8z_torch_cv.yaml
+-rw-r--r--   0        0        0      993 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/8m_torch.yaml
+-rw-r--r--   0        0        0     1509 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/8m_torch_cv.yaml
+-rw-r--r--   0        0        0     1457 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/MMM2_torch.yaml
+-rw-r--r--   0        0        0     1456 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/corridor_torch.yaml
+-rw-r--r--   0        0        0     1515 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/smac/corridor_torch_cv.yaml
+-rw-r--r--   0        0        0     1965 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/test/test_asymmetric_continuous.yaml
+-rw-r--r--   0        0        0     1712 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/test/test_asymmetric_discrete.yaml
+-rw-r--r--   0        0        0     1873 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/test/test_asymmetric_discrete_mhv.yaml
+-rw-r--r--   0        0        0     1401 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/test/test_asymmetric_discrete_mhv_mops.yaml
+-rw-r--r--   0        0        0     1146 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/test/test_discrete.yaml
+-rw-r--r--   0        0        0     1162 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/test/test_discrete_multidiscrete_mhv.yaml
+-rw-r--r--   0        0        0     1301 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/test/test_ppo_walker_truncated_time.yaml
+-rw-r--r--   0        0        0     1205 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/test/test_rnn.yaml
+-rw-r--r--   0        0        0     1829 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/test/test_rnn_multidiscrete.yaml
+-rw-r--r--   0        0        0     1325 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/configs/test/test_rnn_multidiscrete_mhv.yaml
+-rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/distributed/__init__.py
+-rw-r--r--   0        0        0      281 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/envs/__init__.py
+-rw-r--r--   0        0        0     1941 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/envs/brax.py
+-rw-r--r--   0        0        0     2992 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/envs/connect4_network.py
+-rw-r--r--   0        0        0     4505 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/envs/connect4_selfplay.py
+-rw-r--r--   0        0        0     3496 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/envs/diambra/diambra.py
+-rw-r--r--   0        0        0     3116 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/envs/envpool.py
+-rw-r--r--   0        0        0     3195 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/envs/multiwalker.py
+-rw-r--r--   0        0        0     2148 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/envs/slimevolley_selfplay.py
+-rw-r--r--   0        0        0     3690 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/envs/smac_env.py
+-rw-r--r--   0        0        0      279 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/envs/test/__init__.py
+-rw-r--r--   0        0        0      779 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/envs/test/example_env.py
+-rw-r--r--   0        0        0     5217 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/envs/test/rnn_env.py
+-rw-r--r--   0        0        0     1715 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/envs/test/test_asymmetric_env.py
+-rw-r--r--   0        0        0     1596 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/envs/test_network.py
+-rw-r--r--   0        0        0        0 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/interfaces/__init__.py
+-rw-r--r--   0        0        0      674 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/interfaces/base_algorithm.py
+-rw-r--r--   0        0        0      159 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/networks/__init__.py
+-rw-r--r--   0        0        0     1463 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/networks/tcnn_mlp.py
+-rw-r--r--   0        0        0     4860 2023-06-06 12:22:19.334646 rl_games_y-0.0.7/rl_games/torch_runner.py
+-rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 rl_games_y-0.0.7/PKG-INFO
```

### Comparing `rl_games_y-0.0.6/LICENSE` & `rl_games_y-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/pyproject.toml` & `rl_games_y-0.0.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "rl_games_y"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 readme = "README.md"
 authors = [
     "Denys Makoviichuk <trrrrr97@gmail.com>",
     "Viktor Makoviichuk <victor.makoviychuk@gmail.com>",
     "Shengchao Yan <ysc0505@gmail.com>"
 ]
 packages = [
     {include = "rl_games"},
     {include ="rl_games/**/*.py"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.11"
-gym = {version = "^0.24.1", extras = ["classic_control"]}
+gym = {version = "^0.25.1", extras = ["classic_control"]}
 tensorboard = "^2.8.0"
 tensorboardX = "^2.5"
 PyYAML = "^6.0"
 psutil = "^5.9.0"
 setproctitle = "^1.2.2"
 ray = "^1.11.0"
 opencv-python = "^4.5.5"
```

### Comparing `rl_games_y-0.0.6/rl_games/.git/hooks/commit-msg.sample` & `rl_games_y-0.0.7/rl_games/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/hooks/fsmonitor-watchman.sample` & `rl_games_y-0.0.7/rl_games/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/hooks/pre-commit.sample` & `rl_games_y-0.0.7/rl_games/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/hooks/pre-push.sample` & `rl_games_y-0.0.7/rl_games/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/hooks/pre-rebase.sample` & `rl_games_y-0.0.7/rl_games/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/hooks/pre-receive.sample` & `rl_games_y-0.0.7/rl_games/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/hooks/prepare-commit-msg.sample` & `rl_games_y-0.0.7/rl_games/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/hooks/update.sample` & `rl_games_y-0.0.7/rl_games/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/index` & `rl_games_y-0.0.7/rl_games/.git/index`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/logs/HEAD` & `rl_games_y-0.0.7/rl_games/.git/logs/HEAD`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/logs/refs/heads/master` & `rl_games_y-0.0.7/rl_games/.git/logs/refs/heads/master`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/logs/refs/remotes/origin/master` & `rl_games_y-0.0.7/rl_games/.git/logs/refs/remotes/origin/master`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/objects/1b/8cb79243d15f5367053c2e0b6e08ee13486d2e` & `rl_games_y-0.0.7/rl_games/.git/objects/1b/8cb79243d15f5367053c2e0b6e08ee13486d2e`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/objects/1f/721147f878fdca9c3b5dfdcf11fc4194427580` & `rl_games_y-0.0.7/rl_games/.git/objects/1f/721147f878fdca9c3b5dfdcf11fc4194427580`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/objects/7e/42774f9165d4aa805bed4fe49a009ecd448cd8` & `rl_games_y-0.0.7/rl_games/.git/objects/7e/42774f9165d4aa805bed4fe49a009ecd448cd8`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/objects/7e/f78f9e19649c9b3c47d1213b32250a9bf3e388` & `rl_games_y-0.0.7/rl_games/.git/objects/7e/f78f9e19649c9b3c47d1213b32250a9bf3e388`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/objects/83/9143ebf6fc1f117625473c0f843f5186fd5b4c` & `rl_games_y-0.0.7/rl_games/.git/objects/83/9143ebf6fc1f117625473c0f843f5186fd5b4c`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/objects/83/aec7354373d7b6c357a7a726955dd04e575b99` & `rl_games_y-0.0.7/rl_games/.git/objects/83/aec7354373d7b6c357a7a726955dd04e575b99`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/objects/92/300cf5339afc007452ba03a6429fbac560beb7` & `rl_games_y-0.0.7/rl_games/.git/objects/92/300cf5339afc007452ba03a6429fbac560beb7`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/objects/b0/53a46f62fd3debd26a8086221ba4b0b53da81e` & `rl_games_y-0.0.7/rl_games/.git/objects/b0/53a46f62fd3debd26a8086221ba4b0b53da81e`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/objects/c5/83ed29df6ccd6f5b9a415df9d78cf577c922b6` & `rl_games_y-0.0.7/rl_games/.git/objects/c5/83ed29df6ccd6f5b9a415df9d78cf577c922b6`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/objects/c6/8117225b14532206c1fdab9afc9c7f164587cb` & `rl_games_y-0.0.7/rl_games/.git/objects/c6/8117225b14532206c1fdab9afc9c7f164587cb`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/objects/ea/7ad0bc4ca97b0bb110ea383d1885f5d4e512e2` & `rl_games_y-0.0.7/rl_games/.git/objects/ea/7ad0bc4ca97b0bb110ea383d1885f5d4e512e2`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/objects/f9/b97cccad3a3e540b8be03cc28da412957084ad` & `rl_games_y-0.0.7/rl_games/.git/objects/f9/b97cccad3a3e540b8be03cc28da412957084ad`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.idx` & `rl_games_y-0.0.7/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.idx`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.pack` & `rl_games_y-0.0.7/rl_games/.git/objects/pack/pack-17fc9e16c8c0da75db82b39d1ebd8acb84572a42.pack`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/a2c_continuous.py` & `rl_games_y-0.0.7/rl_games/algos_torch/a2c_continuous.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/a2c_discrete.py` & `rl_games_y-0.0.7/rl_games/algos_torch/a2c_discrete.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/central_value.py` & `rl_games_y-0.0.7/rl_games/algos_torch/central_value.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/d2rl.py` & `rl_games_y-0.0.7/rl_games/algos_torch/d2rl.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/flatten.py` & `rl_games_y-0.0.7/rl_games/algos_torch/flatten.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/layers.py` & `rl_games_y-0.0.7/rl_games/algos_torch/layers.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/model_builder.py` & `rl_games_y-0.0.7/rl_games/algos_torch/model_builder.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/models.py` & `rl_games_y-0.0.7/rl_games/algos_torch/models.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/moving_mean_std.py` & `rl_games_y-0.0.7/rl_games/algos_torch/moving_mean_std.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/network_builder.py` & `rl_games_y-0.0.7/rl_games/algos_torch/network_builder.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/players.py` & `rl_games_y-0.0.7/rl_games/algos_torch/players.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/running_mean_std.py` & `rl_games_y-0.0.7/rl_games/algos_torch/running_mean_std.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/sac_agent.py` & `rl_games_y-0.0.7/rl_games/algos_torch/sac_agent.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/sac_helper.py` & `rl_games_y-0.0.7/rl_games/algos_torch/sac_helper.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/self_play_manager.py` & `rl_games_y-0.0.7/rl_games/algos_torch/self_play_manager.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/algos_torch/torch_ext.py` & `rl_games_y-0.0.7/rl_games/algos_torch/torch_ext.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/a2c_common.py` & `rl_games_y-0.0.7/rl_games/common/a2c_common.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/algo_observer.py` & `rl_games_y-0.0.7/rl_games/common/algo_observer.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/categorical.py` & `rl_games_y-0.0.7/rl_games/common/categorical.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/common_losses.py` & `rl_games_y-0.0.7/rl_games/common/common_losses.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/datasets.py` & `rl_games_y-0.0.7/rl_games/common/datasets.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/diagnostics.py` & `rl_games_y-0.0.7/rl_games/common/diagnostics.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/divergence.py` & `rl_games_y-0.0.7/rl_games/common/divergence.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/env_configurations.py` & `rl_games_y-0.0.7/rl_games/common/env_configurations.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/experience.py` & `rl_games_y-0.0.7/rl_games/common/experience.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/experiment.py` & `rl_games_y-0.0.7/rl_games/common/experiment.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/interval_summary_writer.py` & `rl_games_y-0.0.7/rl_games/common/interval_summary_writer.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/ivecenv.py` & `rl_games_y-0.0.7/rl_games/common/ivecenv.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/layers/recurrent.py` & `rl_games_y-0.0.7/rl_games/common/layers/recurrent.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/player.py` & `rl_games_y-0.0.7/rl_games/common/player.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/schedulers.py` & `rl_games_y-0.0.7/rl_games/common/schedulers.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/segment_tree.py` & `rl_games_y-0.0.7/rl_games/common/segment_tree.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/tr_helpers.py` & `rl_games_y-0.0.7/rl_games/common/tr_helpers.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/transforms/soft_augmentation.py` & `rl_games_y-0.0.7/rl_games/common/transforms/soft_augmentation.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/transforms/transforms.py` & `rl_games_y-0.0.7/rl_games/common/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/vecenv.py` & `rl_games_y-0.0.7/rl_games/common/vecenv.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/common/wrappers.py` & `rl_games_y-0.0.7/rl_games/common/wrappers.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_breakout.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_breakout.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_breakout_envpool.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_breakout_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_breakout_envpool_resnet.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_breakout_envpool_resnet.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_breakout_torch_impala.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_breakout_torch_impala.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_gopher.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_gopher.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_invaders_envpool.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_invaders_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_invaders_envpool_rnn.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_invaders_envpool_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_pacman_envpool.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_pacman_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_pacman_envpool_resnet.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_pacman_envpool_resnet.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_pacman_envpool_rnn.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_pacman_envpool_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_pacman_torch.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_pacman_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_pacman_torch_rnn.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_pacman_torch_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_pong.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_pong.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_pong_envpool.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_pong_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_pong_envpool_resnet.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_pong_envpool_resnet.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_space_invaders_resnet.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_space_invaders_resnet.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/atari/ppo_space_invaders_torch.yaml` & `rl_games_y-0.0.7/rl_games/configs/atari/ppo_space_invaders_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/brax/ppo_ant.yaml` & `rl_games_y-0.0.7/rl_games/configs/brax/ppo_ant.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/brax/ppo_ant_tcnn.yaml` & `rl_games_y-0.0.7/rl_games/configs/brax/ppo_ant_tcnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/brax/ppo_grasp.yaml` & `rl_games_y-0.0.7/rl_games/configs/brax/ppo_grasp.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/brax/ppo_halfcheetah.yaml` & `rl_games_y-0.0.7/rl_games/configs/brax/ppo_halfcheetah.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/brax/ppo_humanoid.yaml` & `rl_games_y-0.0.7/rl_games/configs/brax/ppo_humanoid.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/brax/ppo_ur5e.yaml` & `rl_games_y-0.0.7/rl_games/configs/brax/ppo_ur5e.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/brax/sac_ant.yaml` & `rl_games_y-0.0.7/rl_games/configs/brax/sac_ant.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/brax/sac_humanoid.yaml` & `rl_games_y-0.0.7/rl_games/configs/brax/sac_humanoid.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/carracing_ppo.yaml` & `rl_games_y-0.0.7/rl_games/configs/carracing_ppo.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/dm_control/cartpole.yaml` & `rl_games_y-0.0.7/rl_games/configs/dm_control/cartpole.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/dm_control/fish_swim.yaml` & `rl_games_y-0.0.7/rl_games/configs/dm_control/fish_swim.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/dm_control/humanoid_run.yaml` & `rl_games_y-0.0.7/rl_games/configs/dm_control/humanoid_run.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/dm_control/walker_run.yaml` & `rl_games_y-0.0.7/rl_games/configs/dm_control/walker_run.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/dm_control/walker_stand.yaml` & `rl_games_y-0.0.7/rl_games/configs/dm_control/walker_stand.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/dm_control/walker_walk.yaml` & `rl_games_y-0.0.7/rl_games/configs/dm_control/walker_walk.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ma/ppo_connect4_self_play.yaml` & `rl_games_y-0.0.7/rl_games/configs/ma/ppo_connect4_self_play.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ma/ppo_connect4_self_play_resnet.yaml` & `rl_games_y-0.0.7/rl_games/configs/ma/ppo_connect4_self_play_resnet.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ma/ppo_slime_self_play.yaml` & `rl_games_y-0.0.7/rl_games/configs/ma/ppo_slime_self_play.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ma/ppo_slime_v0.yaml` & `rl_games_y-0.0.7/rl_games/configs/ma/ppo_slime_v0.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/minigrid/lava_rnn_img.yaml` & `rl_games_y-0.0.7/rl_games/configs/minigrid/lava_rnn_img.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/minigrid/minigrid_rnn_img.yaml` & `rl_games_y-0.0.7/rl_games/configs/minigrid/minigrid_rnn_img.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/mujoco/ant.yaml` & `rl_games_y-0.0.7/rl_games/configs/mujoco/ant.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/mujoco/ant_envpool.yaml` & `rl_games_y-0.0.7/rl_games/configs/mujoco/ant_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/mujoco/halfcheetah.yaml` & `rl_games_y-0.0.7/rl_games/configs/mujoco/halfcheetah.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/mujoco/halfcheetah_envpool.yaml` & `rl_games_y-0.0.7/rl_games/configs/mujoco/halfcheetah_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/mujoco/hopper.yaml` & `rl_games_y-0.0.7/rl_games/configs/mujoco/hopper.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/mujoco/hopper_envpool.yaml` & `rl_games_y-0.0.7/rl_games/configs/mujoco/hopper_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/mujoco/humanoid.yaml` & `rl_games_y-0.0.7/rl_games/configs/mujoco/humanoid.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/mujoco/humanoid_envpool.yaml` & `rl_games_y-0.0.7/rl_games/configs/mujoco/humanoid_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/mujoco/sac_ant_envpool.yaml` & `rl_games_y-0.0.7/rl_games/configs/mujoco/sac_ant_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/mujoco/sac_halfcheetah_envpool.yaml` & `rl_games_y-0.0.7/rl_games/configs/mujoco/sac_halfcheetah_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/mujoco/walker2d.yaml` & `rl_games_y-0.0.7/rl_games/configs/mujoco/walker2d.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/mujoco/walker2d_envpool.yaml` & `rl_games_y-0.0.7/rl_games/configs/mujoco/walker2d_envpool.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/openai/ppo_gym_ant.yaml` & `rl_games_y-0.0.7/rl_games/configs/openai/ppo_gym_ant.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/openai/ppo_gym_hand.yaml` & `rl_games_y-0.0.7/rl_games/configs/openai/ppo_gym_hand.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/openai/ppo_gym_humanoid.yaml` & `rl_games_y-0.0.7/rl_games/configs/openai/ppo_gym_humanoid.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_cartpole.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_cartpole.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_cartpole_masked_velocity_rnn.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_cartpole_masked_velocity_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_continuous.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_continuous.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_continuous_lstm.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_continuous_lstm.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_lunar.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_lunar.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_lunar_continiuos_torch.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_lunar_continiuos_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_lunar_discrete.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_lunar_discrete.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_multiwalker.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_multiwalker.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_pendulum.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_pendulum.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_pendulum_torch.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_pendulum_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_reacher.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_reacher.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_smac.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_smac.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_walker.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_walker.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_walker_hardcore.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_walker_hardcore.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_walker_rnn.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_walker_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/ppo_walker_tcnn.yaml` & `rl_games_y-0.0.7/rl_games/configs/ppo_walker_tcnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/procgen/ppo_coinrun.yaml` & `rl_games_y-0.0.7/rl_games/configs/procgen/ppo_coinrun.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/10m_vs_11m_torch.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/10m_vs_11m_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/27m_vs_30m_cv.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/27m_vs_30m_cv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/27m_vs_30m_torch.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/27m_vs_30m_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/2m_vs_1z.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/2m_vs_1z.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/2m_vs_1z_torch.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/2m_vs_1z_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/2s_vs_1c.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/2s_vs_1c.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/3m_cnn_torch.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/3m_cnn_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/3m_torch.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/3m_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/3m_torch_cv.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/3m_torch_cv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/3m_torch_cv_joint.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/3m_torch_cv_joint.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/3m_torch_cv_rnn.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/3m_torch_cv_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/3m_torch_rnn.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/3m_torch_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/3m_torch_sparse.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/3m_torch_sparse.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/3s5z_vs_3s6z_torch.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/3s5z_vs_3s6z_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/3s5z_vs_3s6z_torch_cv.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/3s5z_vs_3s6z_torch_cv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/3s_vs_4z.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/3s_vs_4z.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/3s_vs_5z.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/3s_vs_5z.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/3s_vs_5z_cv.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/3s_vs_5z_cv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/3s_vs_5z_cv_rnn.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/3s_vs_5z_cv_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/3s_vs_5z_torch_lstm.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/3s_vs_5z_torch_lstm.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/3s_vs_5z_torch_lstm2.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/3s_vs_5z_torch_lstm2.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/5m_vs_6m_rnn.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/5m_vs_6m_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/5m_vs_6m_rnn_cv.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/5m_vs_6m_rnn_cv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/5m_vs_6m_torch.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/5m_vs_6m_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/6h_vs_8z_torch.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/6h_vs_8z_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/6h_vs_8z_torch_cv.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/6h_vs_8z_torch_cv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/8m_torch.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/8m_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/8m_torch_cv.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/8m_torch_cv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/MMM2_torch.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/MMM2_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/corridor_torch.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/corridor_torch.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/smac/corridor_torch_cv.yaml` & `rl_games_y-0.0.7/rl_games/configs/smac/corridor_torch_cv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/test/test_asymmetric_continuous.yaml` & `rl_games_y-0.0.7/rl_games/configs/test/test_asymmetric_continuous.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/test/test_asymmetric_discrete.yaml` & `rl_games_y-0.0.7/rl_games/configs/test/test_asymmetric_discrete.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/test/test_asymmetric_discrete_mhv.yaml` & `rl_games_y-0.0.7/rl_games/configs/test/test_asymmetric_discrete_mhv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/test/test_asymmetric_discrete_mhv_mops.yaml` & `rl_games_y-0.0.7/rl_games/configs/test/test_asymmetric_discrete_mhv_mops.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/test/test_discrete.yaml` & `rl_games_y-0.0.7/rl_games/configs/test/test_discrete.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/test/test_discrete_multidiscrete_mhv.yaml` & `rl_games_y-0.0.7/rl_games/configs/test/test_discrete_multidiscrete_mhv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/test/test_ppo_walker_truncated_time.yaml` & `rl_games_y-0.0.7/rl_games/configs/test/test_ppo_walker_truncated_time.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/test/test_rnn.yaml` & `rl_games_y-0.0.7/rl_games/configs/test/test_rnn.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/test/test_rnn_multidiscrete.yaml` & `rl_games_y-0.0.7/rl_games/configs/test/test_rnn_multidiscrete.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/configs/test/test_rnn_multidiscrete_mhv.yaml` & `rl_games_y-0.0.7/rl_games/configs/test/test_rnn_multidiscrete_mhv.yaml`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/envs/brax.py` & `rl_games_y-0.0.7/rl_games/envs/brax.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/envs/connect4_network.py` & `rl_games_y-0.0.7/rl_games/envs/connect4_network.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/envs/connect4_selfplay.py` & `rl_games_y-0.0.7/rl_games/envs/connect4_selfplay.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/envs/diambra/diambra.py` & `rl_games_y-0.0.7/rl_games/envs/diambra/diambra.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/envs/envpool.py` & `rl_games_y-0.0.7/rl_games/envs/envpool.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/envs/multiwalker.py` & `rl_games_y-0.0.7/rl_games/envs/multiwalker.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/envs/slimevolley_selfplay.py` & `rl_games_y-0.0.7/rl_games/envs/slimevolley_selfplay.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/envs/smac_env.py` & `rl_games_y-0.0.7/rl_games/envs/smac_env.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/envs/test/example_env.py` & `rl_games_y-0.0.7/rl_games/envs/test/example_env.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/envs/test/rnn_env.py` & `rl_games_y-0.0.7/rl_games/envs/test/rnn_env.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/envs/test/test_asymmetric_env.py` & `rl_games_y-0.0.7/rl_games/envs/test/test_asymmetric_env.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/envs/test_network.py` & `rl_games_y-0.0.7/rl_games/envs/test_network.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/interfaces/base_algorithm.py` & `rl_games_y-0.0.7/rl_games/interfaces/base_algorithm.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/networks/tcnn_mlp.py` & `rl_games_y-0.0.7/rl_games/networks/tcnn_mlp.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/rl_games/torch_runner.py` & `rl_games_y-0.0.7/rl_games/torch_runner.py`

 * *Files identical despite different names*

### Comparing `rl_games_y-0.0.6/PKG-INFO` & `rl_games_y-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl-games-y
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: Denys Makoviichuk
 Author-email: trrrrr97@gmail.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,15 +14,15 @@
 Provides-Extra: envpool
 Provides-Extra: mujoco
 Requires-Dist: AutoROM[accept-rom-license] (>=0.4.2,<0.5.0) ; extra == "atari"
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: ale-py (>=0.7,<0.8) ; extra == "atari"
 Requires-Dist: brax (>=0.0.13,<0.0.14) ; extra == "brax"
 Requires-Dist: envpool (>=0.6.1,<0.7.0) ; extra == "envpool"
-Requires-Dist: gym[classic-control] (>=0.24.1,<0.25.0)
+Requires-Dist: gym[classic-control] (>=0.25.1,<0.26.0)
 Requires-Dist: jax (>=0.3.13,<0.4.0) ; extra == "brax"
 Requires-Dist: mujoco-py (>=2.1.2,<3.0.0) ; extra == "mujoco"
 Requires-Dist: opencv-python (>=4.5.5,<5.0.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: ray (>=1.11.0,<2.0.0)
 Requires-Dist: setproctitle (>=1.2.2,<2.0.0)
 Requires-Dist: tensorboard (>=2.8.0,<3.0.0)
```

