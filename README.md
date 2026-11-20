# ICAN AI Claude Plugin

Plugin chính thức kết nối Claude Code với hệ thống MCP và workflow skills của **ICAN AI** (quản lý giáo trình, mô phỏng HTML, bài tập và đề thi).

## Yêu cầu

- Claude Code CLI đã cài đặt
- Tài khoản ICAN AI (đăng nhập OAuth 2.1 khi kết nối MCP lần đầu; quyền ghi học liệu yêu cầu vai trò `ADMIN` hoặc `MOD`)

## Cài đặt

### Cách nhanh (1 lệnh)

```bash
claude plugin install ican-ai --marketplace zennomi/ican-ai-claude-plugin
```

### Hoặc cài qua 2 bước

```bash
claude plugin marketplace add zennomi/ican-ai-claude-plugin
claude plugin install ican-ai@ican-ai-marketplace
```

Sau khi cài:

1. Mở Claude Code (hoặc chạy `/reload-plugins` nếu đang mở session).
2. Xác thực OAuth với MCP server `ican-ai` khi được yêu cầu.
3. Dùng các skill đi kèm: `/ican-ai:ican-ai-giao-trinh` hoặc `/ican-ai:ican-ai-de-thi`.

## Cập nhật phiên bản mới

Chạy lệnh sau trong terminal:

```bash
claude plugin update ican-ai@ican-ai-marketplace
```

Hoặc bật tự động cập nhật ngay trong Claude Code: chạy `/plugin` → **Marketplaces** → chọn `ican-ai-marketplace` → bật **Auto-update**.
